# Northcoders Data Engineering Katas!

Fork this repository to your own GitHub account because you will be pushing your own solutions to it.

Clone your fork of this repository to your local machine and `cd` into it:

```sh
$ git clone "your fork's URL"

$ cd de-py-katas
```

We are going to use the `make` command to perform some of the standard tasks for this repo. We'll cover `make` in more detail later in the course.

The first task is to set up your **virtual environment**.

Run this command in a terminal:

```bash
make create-environment
```

You should see the `venv` directory appear within the project folder.

Using `make` as described below wil mean you don't have to activate your environment.

After creating your virtual environment, we can install `pytest` by running:

```bash
make pytest
```

The `pytest` library will be used for unit tests. Additionally, there will be `flake8` checks to make sure for PEP8 compliance in the later katas, this will be checked via `make`.

In the terminal, navigate to the root directory of the project, and run:

```
make flake
```

Then, you can use the command below to run your all tests and check for PEP8 compliance:

```
make run-checks
```

Work on the katas and commit changes as needed. When you are happy with your solution, push all your changes to your forked repo. You should push to your fork frequently but as a bare minimum please make sure it's up to date with last week's kata solutions before Monday morning each week:

```sh
$ git push origin main
```

---

## Instructions

This repo is a series of katas to practice your problem solving skills, there is a recommended running order below. There are more katas here than we expect you to complete but have provided extras for you to use as practice once you finish the course to help keep your skills sharp.

**Please start by reading the** `first_python_kata` **and completing** `sentence_to_camel_case`.

---

### Suggested Running Order:

1. sentence_to_camel_case
2. get_distict_letters
3. get_frequencies
4. create_counter
5. lengthen_date
6. get_century
7. years_of_growth
8. herd_the_babies
9. sum_ascii
10. bubble_sort
11. extract_domain_name
12. caesar_cipher
13. roman_numeral_encoder
14. alphabet_position
15. count_bits
16. digital_root
17. fill_square
18. detect_pangram
19. morse_code
20. multiplication_table
21. reduce_by_steps
22. find_partner
23. find_most_repeated
24. vowel_shift
25. alternating_split
26. crack_code
27. binary_search
28. calculate_binary_score
29. justify_line
30. find_the_needle
31. validate_suduko
32. strange_sort
33. gdpr_mask
