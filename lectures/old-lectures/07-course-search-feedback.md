Lab Feedback
============

Process
-------

- Do not [approve PRs that are not in good shape](https://github.com/jncraton/course-search/pull/164#discussion_r2337354473)
- Do not [open feature PRs 44 minutes before a deadline](https://github.com/jncraton/course-search/pull/172). These cannot be properly reviewed.
- Use [imperative mood](https://git.kernel.org/pub/scm/git/git.git/tree/Documentation/SubmittingPatches?h=v2.36.1#n181) in commit messages

Collective Ownership
--------------------

- Everyone owns the whole project

HTML
----

- [Semantic HTML](https://en.wikipedia.org/wiki/Semantic_HTML)
  - [`<label>`](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/index.html#L54) is not appropriate for a table caption

Accessibility
-------------

- Accessibility
  - "Choose a day" dropdown is not properly labeled
  - Sort is not accessible using the keyboard

UX
-----

- [Principle of least astonishment](https://en.wikipedia.org/wiki/Principle_of_least_astonishment) - "If a necessary feature has a high astonishment factor, it may be necessary to redesign the feature."

UX Issues
---------

- Some options take immediate effect, others require the "Apply" button to be pressed
- Most filtering persists over page refreshes, sorting does not
- "CRIM 2510 - The Nature of Crime and Social Deviance" is offered online, but is filtered out of the list of online courses

Style Issues
------------

- A table legend separates various filter options
- Filter controls do not wrap or stack sensibly on mobile
- Table style could be improved
- White gaps are present between table columns
- Content feels crowded and thrown together

Code Quality
------------

- Why does [currentCourses](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L12) exist as a global?
- Why have a [wrapper function to set a global variable](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L126-L129)?
- Perhaps data should be cleaned up or pre-processed once instead of using [getDept](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L15) and [daysCount](https://github.com/jncraton/course-search/blob/e1e7162f7916cc48574bcad45ae635589f790f88/main.js#L18-L23)
- [Event Handlers](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L134-L153) seem needlessly complex. Should you just call `renderTable` if any input changes?


Code Quality
------------

- A common UI element (dropdown menu) is rebuilt from scratch in a way that does not support accessibility
  - A global [sortMode](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L13) is not necessary if we use a dropdown
- [Sorting](https://github.com/jncraton/course-search/blob/838c29d5877b3e3cb501a1ef83019db36a869819/main.js#L79C1-L102C4) doesn't feel very [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)

Regression
----------

- Re-open [liberal arts filter](https://github.com/jncraton/course-search/issues/167)
- Current implementation filters by courses that have liberal arts in the name only and does not satisfy the requirements of the story

Regression
----------

- Online filtering should exactly match value found in the "Format" column

New Issues
----------

- All `input` elements should have appropriate associated labels

New Issues
----------

- Column headings should be used for sorting where appropriate

New Issues
----------

- Table should be appropriately formatted
    - Left align text
    - Center align numbers
    - Align titles with data
    - [Web Typography: Designing Tables to be Read, Not Looked At](https://alistapart.com/article/web-typography-tables/)
    - [Clear off the table](https://www.darkhorseanalytics.com/blog/clear-off-the-table)

New Issue
---------

- Style the page appropriately
  - You all are not professional designers, but you can do better than this
  - Consider the basics (proximity, alignment, repetition, contrast)

Pair Programming
----------------
