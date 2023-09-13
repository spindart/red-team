# What are regular expressions?

Regular expressions (or Regex) are patterns of text that you define to search documents and match exactly what you're looking for.

# Why should I learn how to use them?

Even if you won't need them sooner or later, it's a great tool to know how to use. It will make you more capable in CTF's, and potentially a better developer if that's a goal you have. You spend a little time learning it and save yourself lots of time in the long run by using it.

# I know all that, but I'm lazy.

This is a lazy person's tutorial. There's a little reading, and then you learn by doing.

# Where's the 'Deploy' button?

There's no machine to deploy. There are two ways to test your expressions. Either:

* create a text file with some test paragraphs (in a Unix machine) and then use egrep <pattern> <file> to see what matches and what doesn't, or
* use an online editor like https://regexr.com/. You can add your own text in the "Text" field, and then type your expressions (patterns) in the "Expression" field.

Another editors: 

https://regex101.com/


# Charsets

When searching for a specific string in a file or block of text, you can search for it as is, with `grep 'string' <file>` . But what happens if you want to search for patterns of text? For example, you could be looking for a word that starts with a specific letter, or any words that end with numbers. That's where Regular Expressions come in.

Both of the aforementioned problems can be solved by using charsets. A charset is defined by enclosing in `[` square brackets `]` the character(s), or range of characters that you want to match.  Then, it finds every occurrence of the pattern you have defined in the file/text you are searching.

`[abc]` will match <b>a, b, and c</b> (every occurrence of each letter)

`[abc]zz` will match <B>azz, bzz, and czz</b>.

You can also use a `-` dash to define ranges:
`[a-c]zz` is the same as above.

And then you can combine ranges together:
`[a-cx-z]zz` will match <B>azz, bzz, czz, xzz, yzz, and zzz</b>.

Most notably, this can be used to match any alphabetical character:
`[a-zA-Z]` will match any single letter (lowercase or uppercase).

You can use numbers too:
`file[1-3]` will match <b>file1, file2, and file3.</b>

Then, there is a way to exclude characters from a charset with the ^ hat symbol, and include everything else.
`[^k]ing` will match <b>ring, sing, $ing, but not king</b>.

Of course, you can exclude charsets, not just single characters.
`[^a-c]at` will match <b>fat and hat, but not bat or cat</b>.

Note 1: Don't confuse strings with charsets. The charset `[abc]` will match the string `abc`, but also `cba` and `ca`. It doesn't match the string, but rather every occurrence of the specified characters in that string.

Note 2: When specifying charsets, you should type the letters in the same order they appear in the questions, to avoid typing something correct that is not the right answer.

Note 3: Answering some of these questions is going to be tricky. Often times there are many different patterns that match specific strings. That means (as stated in the previous note) that you may find a proper solution that isn't the right answer for this room (because there can only be one). The right answer is typically the most efficient regex for that question. Efficient in this context means 2 things:
*  Be specific. Here's an example: you could match any character from a to c using the `[a-z]` charset. But if the question only requires you to match characters from `a` to /`c`, you should use the `[a-c]` charset, not `[a-z]`.
* Don't be too specific. In contrast to the previous example, if a question requires you to match `a, c, f, r, s, z`, at that point, the expression that matches those specific characters would get longer and more complicated. So, it would make more sense to use `[a-z]`, because it is short and simple.