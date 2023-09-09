# CSE 150 Lecture Notes

Currently maintained by Jeffrey Jiang. 

## Access

You can build the latex yourself, but the compile PDF can always be found [here](build/lectures.pdf).

## Contribution

Let me know if you are interested in contributing to this repository. 

The main content is stored in the [chapters](src/chapters/) directory. Each $\LaTeX$ file is named based on the date the lecture takes place in ISO 8601. The benefit of this system is that the lecture files are sorted automatically by the day in which the lecture occur. 

Each $\LaTeX$ file should begin with the following:

```latex
\chapter*{Lecture \arabic{lecturenum}}
\addcontentsline{toc}{chapter}{Lecture \arabic{lecturenum}}
\addtocounter{lecturenum}{1}
```

After that, you can write up the notes. However, some things to note:

- Prefer to use `\(STATEMENT\)` over `$STATEMENT$`
- Prefer to use `\[STATEMENT\]` over `$$STATEMENT$$`
- Try to keep the formatting consistent between all files.
- Do not add auxiliary files to the repository. The [.gitignore](.gitignore) should deal with most of these issues. Additionally, keep auxiliary files in [build](build).