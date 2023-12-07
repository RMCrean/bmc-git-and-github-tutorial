## Hands on Session - Part 3, Branches and Merging

- **Recap: Branch** Branching lets you have different versions of a repository at one time. By default, your repository has one branch named `main` (sometimes called `master` instead) that is considered to be the definitive/central branch. Typically a new branch is used to work on new features or bug fixes without affecting the main codebase until you are ready to merge the changes.

- **Recap: Merge** Merging combines changes from different branches into a single branch, typically changes are merged into the `main` branch.

![git branching and merging visualised](../assets/git_branches_merging_not_mine.png)
<sub><sup>Image taken from coderefinery: https://coderefinery.github.io/git-intro/branches/ </sup></sub>

---

## Part 3.1, Create a New Branch:

Now we'll create a new branch inside our repository. 


```
git branch new-feature main
```

This means we'll create a new branch called `new-feature` using a copy of the current state of the `main` branch. 

Now if we run:
```
git branch 
```

We'll see two branches, and the branch we are working on (main) indicated by an asterisk.

To swap to the other branch we can do: 

```
git checkout new-feature
```

If you now run `git branch` again, you'll now see we're working in the `new-feature` branch. 


Tip: you can combine the creation of a new branch and swapping to the branch is a single step:
```
git checkout -b new-feature main
```

---

## Part 3.2, Make some commits in the new branch and merge them. 


---

## Part 3.3, TODO.



---

## Part 3.4, TODO.


---

## Part 3.5, TODO.



---

## Appendix

### Practical Tips:

- Where do I store my projects? I have a folder called projects close to the root folder of my pc (TODO add pic). All projects get there own folder and I clone them to here.

- [Undoing things tutorial](ttps://git-scm.com/book/en/v2/Git-Basics-Undoing-Things)

- Use GitHub or something like VSCode to create your initial repository rather than Git directly. This will give you the chance to add things like .gitignore files and a License file.

- Use a .gitignore file to handle large data files or sensitive information you don't want to include. (As we saw, these can be created automatically when you make a repository with GitHub or VSCode, with good defaults for a project involving for example: python or R).

- Commit regularly, it will make your life easier. 


### Other Ways to Share Research Data
- Raw research data, associated with a paper, especially large data files are probably better shared using a service like [Zenodo](https://zenodo.org/).
- There is nothing wrong with having both a GitHub repository and a Zenodo page for your project.


### GitHub Alternatives
As you hopefully now appreciate, you don't need to use GitHub to make use of Git. Alternative places to host remote repositories include for example [bitbucket](https://bitbucket.org/product/) and [GitLab](https://about.gitlab.com/) and they tend to offer very similar functionality.
