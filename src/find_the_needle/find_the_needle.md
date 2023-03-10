# find_the_needle

Find the needle(s) in a haystack by creating a function that returns all properties (recursively) which contains the needle (string).

The return value should be an **alphabetically sorted list** with dot notation 'path' for each mention of the string (see below examples).

- It should not care if the needle is capitalised or not.
  For example it should find "curry" in the haystack if the needle is "Curry".
  In this case it is ok to ignore "cuRRy"

- The results do not need to be entire words. In the above case it would find "Curry" in the string "Our website is http://www.awesomecurry.com"

## Examples

```py
haystack = {
	name: "Northcoders",
	description: "Awesome coding bootcamp",
	staff: {
		tutors: "James and Chris",
		support: "Louise"
	},
	contactDetails: {
		web: "https://northcoders.com",
		phone: "",
		address: {
			office: "Northcoders, Gold 67, The Sharp Project, Manchester",
			postcode: "M40 5BJ"
		}
	},
	reviews: {
		april: {
			chris: "I love Northcoders",
			james: "It is awesome!"
		},
		may: {
			louise: "Northcoders is a fantastic coding bootcamp"
		}
	}
};
```

```py
needle = "Sausages";
needleHaystack(haystack, needle);
# []
```

```py
needle = "m40";
needleHaystack(haystack, needle);
# ["contactDetails.address.postcode"]
```

```py
needle = "coding";
needleHaystack(haystack, needle);
# ["description", "reviews.may.louise"]
```

```py
needle = "NorThcOdErs";
needleHaystack(haystack, needle);
# ["contactDetails.address.office", "contactDetails.web", "name", "reviews.april.chris", "reviews.may.louise"]
```
