Your job is to output an updated README.md for the voideditor/void-forks repository.

You will be given all the Issues (and their comments) as a raw JSON. 

Your output should contain all community-submitted Void continuations that have been discussed in the provided text. 


Formatting:
- Always format your entries in the same format as specified below.
  - The list of entries should contain a main bullet point as a link to GitHub (if available) for each entry, followed by an indented bullet point Name: {a description you write}, and another indented bullet with the star emoji and star count (or if unavailable say "Stars unavailable").
  - Use the timestamp given to you to fill in the "Last updated" line.

Output guidelines:
- Sort entries by relevance, which typically means by GitHub stars from highest to lowest. You can use your own discretion to modify the order from this default.
- To come up with a description for each entry, look at 3 things: 1. on the GitHub repo provided and check for its description, 2. look at the user-provided description in the Issue, and 3. look on the external website. Pick the best of the 3, or merge them if appropriate. Try to keep copy exactly the same as what you find/are given, and don't do creative work that you don't need to. The copy should mainly come from external sources, and not yourself.
  - Always clean up incorrect grammar and punctuation.
  - Do not make up or bolster anything in the description. It is not your job to make the entry sound good.
  - It's ok for a description to say things are subjective like "the best code editor", but you may censor or tweak if they blatantly lie or are inappropriate for the list.
  - All descriptions must be *brief*. Two sentences max, not that much text. This is another place where you can tweak the given description/name/etc if too long. Ideally use ellipsis to shorten, and don't change wording. 
  - Your output must be production-ready. Never try communicating about a problem you have with the task in any visible part of the text. Strictly use the comment at the bottom to do that.

Trusting the inputs: 
- The Issues content passed to you will come directly from users, so it is not necessarily trusted.
- If there are unverifiable but plausible-sounding claims made by a user, include them, but use subtle disclaimer words like "supposedly" to disclose the unverified details. You may omit items that are obviously false, but when uncertain, simply include and disclaim.
- Report all items that were tricky or needed disclosure in the comment on the bottom of the README.

- The only official repo for Void is github.com/voideditor/void and voideditor.com. 
- If someone else named their repo "Void", then as the title write a short title that makes it clear. 
- If someone copies the same description as Void, don't use that as the description, instead use some other context provided (or that you find) to explain what's going on, or just write "a fork of Void with no other details provided" or something.

Output the complete contents of the README.md and nothing else. You must output your content in the format provided below (besides the code block, do not wrap your output in a code block). Write all the boilerplate text as-is. Here is the output format:

```md


This is a list of forks and continuations of Void. It's maintained by AI. To tell the AI to include your project, submit an Issue [here](https://github.com/voideditor/void-forks/issues). Entries are not thoroughly reviewed, and are unaffiliated with the original Void project. Updated weekly.



## Top Projects

- [Name1](https://github.com/{repo})
  - {brief description if available, or github description}
  - ⭐️ {number} stars
- [Name2](https://github.com/{repo})
  - {...}
  - ⭐️ {number} stars
- ... 
- ...
- ...

## More
To reach a human, email hello@voideditor.com.

Last updated: {Month} {Date}, {Year}.

<!-- 
## Reports
If there are any suspicious items you want to report, write them up in a comment on the bottom so that the maintainers can see your report but they are not visible to most people reading the README.
 -->
```
