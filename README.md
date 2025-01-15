<!--
create a software
pytohn: no input()

https://matt.might.net/articles/shell-scripts-for-passive-voice-weasel-words-duplicates/
"How to Write Mathematics" by Paul R. Halmos and "Mathematical Writing" by Donald E. Knuth
https://www.gnu.org/software/diction/
https://vale.sh/
https://github.com/FusionAuth/fusionauth-site/blob/main/.github/workflows/vale.yml

Formatting:
https://web.cs.ucdavis.edu/~rogaway/papers/moral.html
https://blog.cr.yp.to/20241028-surveillance.html
https://blog.cr.yp.to/
https://danluu.com/nothing-works/

Classic Essays:
https://www.gnu.org/philosophy/right-to-read.en.html
-->

# Programmer English

Programmers have developed a dialect of English distinct from [standard American English](https://en.wikipedia.org/wiki/Standard_American_English).
This document lists some features of this dialect.
<!--
By recognizing these features you can better identify "true programmers",
and by adopting these features into your own language use you can be perceived by others to be a "true programmer".
-->

This document covers:

1. [Phonology](#Phonology)
1. [Lexicon](#Lexicon)
1. [Grammar](#Grammar)
    1. [In Natural Language](#Grammar)
    1. [In Markdown](#Markdown)
    1. [In Python](#Python)
1. [Discourse](#Discourse)

## Phonology

Abbreviations are pronounced as acronyms whenever possible.
That is, they are read as words and not letters.

1. RAG is pronounced "rag" not "R-A-G".

    > **NOTE:**
    > The word "rag" has only one sylable and is faster/easier to pronounce than the 3-sylable "R-A-G".
    > The practice of pronouncing abbreviations as acronyms stems from the programmer's desire for efficiency in all things.

1. ICLR is pronounced "I clear".

1. PNG is pronounced "ping" and not "pee-en-gee".
    This pronunciation is [specified in the standard](https://www.w3.org/TR/2003/REC-PNG-20031110/#1Scope).

    The G in GIF is pronounced like the G in GIGANTIC.

    > **NOTE:**
    > It is acceptable to say the letters of these acronyms if you are reading the name of a file.
    > For example, it is okay to pronounce `test.png` as "test dot pee en gee".
    >
    > This stems from the fact that some file formats have two different extensions that can be pronounced the same (like `.jpg` and `.jpeg`).
    
    <!--
    > The filename `test.py` is normally read "test dot pie" and not "test dot pee why".
    -->

1. SQL is pronounced "sequel" and not "ess-que-ell".

    > **NOTE:**
    > The [original name of the SQL programming language was SEQUEL](https://en.wikipedia.org/wiki/SQL#History),
    > but due to copyright reasons the authors shortened the name by removing the vowels.

    > **NOTE:**
    > Saying "an SQL" is a moderately common in-joke for technical incompetence.
    > 
    > <img width=400px src=img/dilbert.gif />
    >
    > On the other hand, the most commonly used database in the world is sqlite3,
    > and the documentation consistently uses the phrase "an sqlite database".
    > The [documentation for MySQL](https://dev.mysql.com/doc/refman/5.7/en/what-is-mysql.html) specifies that the pronunciation is "My Ess Que Ell".
    > But both of these documents are wrong.

    > **NOTE:**
    > It is expected that programmers will have strong opinions about contentious issues.
    > The fact that a programmer is using strong language suggests that the issue is actually highly contentious.

1. Common exceptions include:
    1. HTML is pronounced "H-T-M-L" and CSS is pronounced "C-S-S".
        Notice there are no vowels in these names that allow them to be shortened.

    1. IP is pronounced "I-P" and ISO is pronounced "I-S-O".
        These abbreviations contain vowels, but the natural pronounciation does not correspond to an English word, and so the letters are pronounced to avoid ambiguity.

Sometimes words are pronounced contrary to standard pronunciation rules of English for etymological reasons.
Sometimes words are pronounced contrary to standard pronunciation rules as an explicit [shibboleth](https://en.wikipedia.org/wiki/Shibboleth).
Sometimes the reason is a mixture of both.

<!-- logit != lojit; nginx, gunicorn, pypi, "insights", outputted/output ; AdaBoost vs ADA-->

1. Regex is pronounced with a hard G.

    (The word "regex" is a shortened form of *regular expressions*, and "regular" is pronounced with a hard G.
    The temptation to use a soft g is due to the fact that [most English words of Latin/Greek descent that have a G followed by an E use a soft E, combined with the fact that most techincal words in English come from Latin/Greek.)

1. Logit is pronounced with a soft g and short i.  (Like "logic with a t" not "Lowe git".)

    (The word [logit](https://en.wiktionary.org/wiki/logit) is a [portmantaeux](https://en.wikipedia.org/wiki/Blend_word) of the words *logistic* and *bit*.
    It should therefore be pronounced with the same sounds as logistic. 
    The temptation to use a hard g/long o comes from the standard English pronunciation rules.)
    <!-- see how legit is pronounced -->

1. GNU is pronounced with a hard G.

    (There is no good reason for this one other than to make identifying outsiders easy.
    See the [official documentation](https://www.gnu.org/gnu/pronunciation.en.html).)

    The GNOME desktop [is pronounced with a hard G](https://stuff.mit.edu/afs/athena/astaff/project/aui/html/pronunciation.html) because the G in GNOME stands for GNU.

    The command-line plotting software gnuplot is [not affiliated not affiliated with GNU](http://www.gnuplot.info/faq/faq.html#x1-70001.2) and so the G is silent.

    The gunicorn webserver is not affiliated with GNU but [still pronounced with a hard G](https://github.com/benoitc/gunicorn/issues/139) because the G stands for green.

1. Latex is pronounced "La-tech" and not "La-techs".

    The "tex" comes from the greek root τεχ [from wence](https://english.stackexchange.com/questions/10906/is-from-whence-correct-or-should-it-be-whence) we get the word "technology".
    The "x" is actually a greek chi which is pronounced most similarly to "k" in English.

    > **NOTE:**
    > Latex is derived from TeX, which was invented by Donald Knuth.
    > Knuth pronounces the K in his last name.

Computer science was historically a branch of mathematics.
Programmers treat mathematical notation with respect and pronounce it properly.

1. Math symbols are pronounced using their corresponding latex code.
    For example:

    | symbol        | latex code    | pronunciation |
    | ------------- | ------------- | ------------- |
    | $\mathcal X$  | `\mathcal X`  | mathcal X     |
    | $\bar X$      | `\bar X`      | bar X         |
    | $\cup$        | `\cup`        | cup           |

1. Greek letters should all be pronounced correctly.
    The only exception is $\pi$ which is pronounced "pee" in Greek but "pie" in mathematics to distinguish it from the English "p".

    See [this fun song](https://www.youtube.com/watch?v=749JoaGOCcg) for correct pronunciation examples.

## Lexicon

Words have precise meanings, and their use should reflect those precise meanings.

1. The word "code" is a collective noun when it refers to computer code.

    > Incorrect: I used VSCode to write the python **codes** for my website.
    > 
    > Correct: I used VSCode to write the python **code** for my website.

    "Code" is not a collective noun when it is used as a synonym for creditials / passwords.

    > Correct: I entered my login **codes** for the bank.
    > 
    > Note that the use of the plural implies that more than one password was needed.

1. The word "literally" should not be used metaphorically.

    > Incorect: I literally spent one thousand hours on the homework assignment.

1. The word "exponentially" should only be used in reference to functions that actually grow exponentially.

    > Incorrect: $O(n^3)$ grows **exponentially**.
    > 
    > Correct: $O(n^3)$ grows **polynomially**; $O(3^n)$ grows exponentially.

1. The word "random" should not be used as a synonym for "arbitrary."
    In particular, it should only be used when there is a corresponding distribution that is being sampled from.

    > Incorrect: The parameter to python's `print` function can be any **random** string.
    >
    > Correct: The parameter to python's `print` function can be any **arbitrary** string.

<!--
Non-technical jargon should never be used.

1. Programmers rarely verb nouns.
    We do not give an "ask"
    When we hear these phrases, [it's definitely an annoy](https://news.ycombinator.com/item?id=42714775#42716628).
-->

Mistakes with big-Oh notation are extremely common.
They are a sure sign that the author is an amateur and not to be taken seriously.

1. Every computer scientist should be familiar with $O$, $\Omega$ and $\Theta$ notation.
    This means having the definitions memorized and being able to apply the definitions with easy to simplify functions.
    [Wikipedia has an excellent summary.](https://en.wikipedia.org/wiki/Big_O_notation#Family_of_Bachmann%E2%80%93Landau_notations)

1. A common mistake is to assume that big-Oh notation is only used for the runtimes of algorithms.

    > Incorrect: Matrix multiplication is $O(n^3)$.
    >
    > Correct: **The runtime** of matrix multiplication is $O(n^3)$.  The space complexity of matrix multiplicaiton is $O(1)$.

1. A related mistake is not fully specifying the function that the big-Oh notation is simplifying.

    > Incorrect: The $n\times n$ identity function is $O(n)$.
    >
    > Correct: **The number of non zeros** in the $n\times n$ identity matrix is $O(n)$.

1. Big-Oh notation should not be used as a synonym for "approximately" when plugging in constants.

    > Incorrect: If $d_{VC} = \Theta(d)$ and $d=100$, then $d_{VC} = \Theta(100)$.
    >
    > Correct: If $d_{VC} = \Theta(d)$ and $d=100$, then $d_{VC} \approx 100$.

## Grammar

Programmers are used to writing programming languages with strict grammar.
Therefore, they write their prose also observing strict grammar rules.

American programmers tend to follow [British grammar rules](https://www.unr.edu/writing-speaking-center/writing-speaking-resources/british-american-english) when they are "more logical".
Examples include: placing punctuation outside of quotation marks, using YYYY-MM-DD time formats, and the [Oxford comma](https://en.wikipedia.org/wiki/Serial_comma).
(Clever placement of examples is common, as are parentheses (and doubly nested parentheses).)

Note the careful placement of the period in the last sentence above.
Also note that this sentence and the previous were written in the 2nd person imperative tense.
Programmers expect the reader to participate actively in reading and commonly command their reader to perform certain tasks.

### Markdown

Use code blocks properly.

1. Inline code (single backticks) are for including names of functions (`print`), variables (`foo`) or other short code snippets in text.

1. Code blocks (triple backticks) are for including full commands.
    ```
    for i in range(10):
        print(i)
    ```
    Note that even if you have a one line code snippet, it should be contained in a code block.
    The following is incorrect

    `print(i)`

    and the following is correct

    ```
    print(i)
    ``` 

Never take screenshots of text (especially code or error messages).
1. Google will not index screenshots.
1. End users cannot copy/paste a screenshot.
1. Long error messages often fill multiple screens, and a screenshot will truncate the error.

Code that is typed into a prompt should include the prompt in the code block.

1. This allows us to know at a glance

    1. what program the code is being entered into, and
    1. which parts of the code block are code and which parts are the code's output.

1. For example:

    ```
    >>> print('hello world')
    hello world
    ```

    ```
    $ echo "hello world"
    hello world
    ```

    ```
    sqlite> SELECT 1;
    1
    ```

Write one sentence per line.
(View the source of this markdown file for examples.)
1. [This will improve the quality of your English.](https://sive.rs/1s)
1. [This will make your git diffs nicer.](https://rhodesmill.org/brandon/2012/one-sentence-per-line/)
1. [This will make navigating in vim faster.](https://vi.stackexchange.com/a/2368)

### Python

All python programmers should follow [PEP8: Style Guide for Python Code](https://peps.python.org/pep-0008/) and [PEP20: The Zen of Python](https://peps.python.org/pep-0020/).

1. Variables should be named in `snake_case` and not in `CamelCase` because python is a snake.

1. Operators should be surrounded by a space like `1 + 1` and not `1+1`.

1. Automated tools like `flake8` should be used to verify compliance.

    It is okay to manually override some of the rules if have a compelling reason.
    For example, it is very common to not obey the 80 character per line limit.

All functions should have test cases.
If a function does not have a test case, it should be assumed to be incorrect.

1. The only exception to this rule is functions doing IO.
    Test cases are often awkward/difficult for these functions.

1. A corollary is that no function should do both IO and logic processing.
    Functions should be split so that the logic processing can be easily tested with test cases.

Code should be broken up into "paragraphs", and each paragraph should have a "topic sentence comment".
The comment should be written in the second person (i.e. a command).

1. Here is an example of some data processing code
    ```
    # one hot encode categorical columns
    df = pd.get_dummies(df)
    print(f"df.shape={df.shape}")

    # convert non-numeric columns to numeric
    le = sklearn.preprocessing.LabelEncoder()
    df = df[df.columns[:]].apply(le.fit_transform)
    print(f"df.shape={df.shape}")

    # apply the polynomial feature map
    poly = sklearn.preprocessing.PolynomialFeatures(3)
    df = poly.fit_transform(df)
    print(f"df.shape={df.shape}")

    # apply a random projection
    proj = sklearn.random_projection.GaussianRandomProjection(
        n_components=120,
        random_state=42,
        )
    df = proj.fit_transform(df)
    print(f"df.shape={df.shape}")
    ```

1. The imperative is used for two reasons:
    1. Programmers command computers to do our bidding.
        We do not document the behavior of computers following their own volition.
    1. The 2nd person English imperative is shorter than other tenses in English because there is no need to write the subject of the verb.
        Programmers prize efficiency and so take advantage of the ability to not write/read the noun.

1. If longer comments are needed, or the comment doesn't naturally fit into the 2nd person, then the comment should be annotated with a `NOTE`.

    ```
    # NOTE:
    # This is an example of how to write a non-imperative comment.
    # Notice that I still write one sentence per line.
    ```

## Discourse

[Hubris is one of the three virtues of a programmer.](https://thethreevirtues.com/)
But you must be humble when describing your projects.
1. When Linus Torvalds announced Linux to the world, he said:

    > I'm doing a (free) operating system (just a hobby, won't be big and professional like gnu) for 386(486) AT clones.
1. It is okay to lose your humility after proving your software is *world class*.

    For example, the sqlite3 database contains a [full page documenting how it is the most deployed piece of software ever developed](https://www.sqlite.org/mostdeployed.html).
    This is an okay "brag" because [the author](https://en.wikipedia.org/wiki/D._Richard_Hipp) can easily prove it.

Programmers correct each others' mistakes.
1. If you point out that I made a mistake, I see it as a compliment and not an insult.
    It means that you cared enough about my writing to actually have read and thought about it.
1. If you see a mistake in this document (or want to add more),
    then please submit a pull request.

The purpose of writing is to communicate complex ideas so that they are easy to understand.
1. The purpose is NOT to impress a humanities professor.
1. Many of your readers will be non-native English speakers.
1. All of your readers have other things to do with their time.

Writing should be information dense.
1. Avoid unneeded adjectives.
1. Your writing should not sound like ChatGPT.

    [Recent research](https://arxiv.org/abs/2406.07016) has identified a number of words commonly used by LLMs.
    They include:
    meticulously, delving, intricate, comprehensive, significant, pivotal, accentuating.

    Notice that these are all either "unneeded adjectives" or "not humble".

Concrete techniques for making your writing easy to understand include:
1. Make your content easily skim-able by using numbered lists, headers, and other markdown features.
1. Use few words, not many words.
1. Use little words, not big words.
    1. Prefer "use" to "utilize".
    1. Prefer [Germanic words to French/Latin words](http://www.csun.edu/science/ref/language/german-latin-english.html).
1. Focus on examples.
    1. It is also important to include "general principles" and "high level ideas".
    1. But they should be explained via examples.
    1. LLMs learn only through examples; humans learn "mostly" through examples.
