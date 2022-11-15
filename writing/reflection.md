# Contact Searching

TODO: Make sure that you delete all of the TODO markers and the written prompts
from this document. You should also ensure that the document does not have any
mistakes in spelling, grammar, or the syntax of Markdown. Ultimately, the final
version of your reflection should be a polished document that is suitable for
publication on your web site.

## Andrew Briercheck

## Program Output

### What is the output from running the following commands?

```
andrewbriercheck@Deep-Thought contactsearcher % poetry run contactsearcher --job-description "engineer" --contacts-file input/contacts.txt
Traceback (most recent call last):
  File "<string>", line 1, in <module>
  File "/opt/homebrew/Cellar/python@3.10/3.10.6_2/Frameworks/Python.framework/Versions/3.10/lib/python3.10/importlib/__init__.py", line 126, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
  File "<frozen importlib._bootstrap>", line 1050, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1027, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1006, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 688, in _load_unlocked
  File "<frozen importlib._bootstrap_external>", line 883, in exec_module
  File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
  File "/Users/andrewbriercheck/Documents/Schoolwork/Senior_Year/CMPSC102/08_survey_contact_searching-Burnytoast/contactsearcher/contactsearcher/main.py", line 7, in <module>
    from search import search_for_email_given_job
```
- `poetry run contactsearcher --job-description "engineer" --contacts-file input/contacts.txt`

```
andrewbriercheck@Deep-Thought contactsearcher % poetry run contactsearcher --job-description "neer" --contacts-file input/contacts.txt 
Traceback (most recent call last):
  File "<string>", line 1, in <module>
  File "/opt/homebrew/Cellar/python@3.10/3.10.6_2/Frameworks/Python.framework/Versions/3.10/lib/python3.10/importlib/__init__.py", line 126, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
  File "<frozen importlib._bootstrap>", line 1050, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1027, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1006, in _find_and_load_unlocked
  File "<frozen importlib._bootstrap>", line 688, in _load_unlocked
  File "<frozen importlib._bootstrap_external>", line 883, in exec_module
  File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
  File "/Users/andrewbriercheck/Documents/Schoolwork/Senior_Year/CMPSC102/08_survey_contact_searching-Burnytoast/contactsearcher/contactsearcher/main.py", line 7, in <module>
    from search import search_for_email_given_job
ModuleNotFoundError: No module named 'search'
```
- `poetry run contactsearcher --job-description "neer" --contacts-file input/contacts.txt`

## Source Code and Configuration Files

### Describe in detail how your provided source code works

#### The source code statement that makes the `search` module available to `main`


```
import typer
from search import contacts
from search import search_for_email_given_job
from rich.console import Console

cli = typer.Typer()
console = Console()
```

This module begins by importing typer into the project. Once the 

#### The source code statement that extracts the current job description for a contact

```

```
TODO: Write at least one paragraph to explain the request source code

#### Invocation of the function called `search_for_email_given_job`

```

```
TODO: Write at least one paragraph to explain the request source code

#### Test case for the function called `search_for_email_given_job`

```

```
TODO: Write at least one paragraph to explain the request source code

#### Execute trace of the `contactsearcher` program

```

```
TODO: Write at least one paragraph to explain every function call when running `contactsearcher`

TODO: Your discussion should start with the invocation of the `contactsearcher`
function in the `main` module, explain all of the subsequent function calls in
the correct order, and then show how the program's control returns to the
`contactsearcher` function in the `main` module.

- `poetry run contactsearcher --job-description "engineer" --contacts-file input/contacts.txt`

## Professional Assessment

### So far this semester, what is one area in which you have struggled? How did you overcome this challenge?

The biggest thorn in my side at the moment appears to be importing things. The major error that was hanging everything else up appeared to be my ability to import the function and the list from "search". This seems to be an issue I'm having a lot and I'm getting a bit frustrated by it >_<.


### Based on your experiences with this project, what is one way in which you want to improve?

I need more experience with different data types. I'm getting much more confident with how lists work, dictionaries still feel a little foreign, but they are slowly making more sense. Sets are making some sense, but trying to run this through as a set was confusing, as I'm still trying to get it to cooperate in the way I needed it to. 