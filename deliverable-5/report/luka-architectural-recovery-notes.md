## TODO
- [ ] Do we add package.json references as a secondary module view?
- [ ] Better explanation of why it is smart to keep folder structure in module view
	- [ ] Better overview (easier to navigate)
	- [ ] Clusters nodes around folder, which makes it easier to see references crossing folders (not necessarily a problem)
- [ ] Do we add test coverage and code-churn metrics?
- [ ] Proof read
- [ ] Get it below 5 pages

1. Introduction (0.5)
2. Methodology (1)
3. Results (1.5)
4. Discussion (1.5)
5. Appendix (does not count in)

## 1. Introduction
Length: 0,5754166667

## 2. Methodology
Length: 1,6458333333

## 3. Results
Length: 1,5608333333

## 4. Discussion
Length: 1,5970833333

Total: 5,3816666667

## Pages Sum


### Strong points (What Worked)
- Interactivity of the diagram

### Weak points (Do better?)
- Only static analysis
- Slow to decide on goal (might not be good)
- Unused references are still shown
- TODO

### Limitations
- Metrics problem
	- Code time changes, line changes, etc
- Module references and how we should probably add them

### Original Version
#### Strong Points Of The Architectural Recovery

One strong point of this reconstruction is the interactive module view. Whenever work has to be done on unfamiliar code, a lot of time is spent navigating the file system, following references and manually stepping through the code in debug mode. By having a dependency graph next to the code in the form of a module view, allows the developer to filter for two specific sub folders, and see exactly how they reference each other. This makes architectural decisions made more clear and the interactivity, moving- and removing nodes, is a more natural way of interacting with code.

While Python, especially combined with Jupyter Notebooks, are a fantastic tool due to the ease of use but the visualization options are quite lacking compared to nodejs. In future if Jupyter Notebooks for nodejs becomes more stable, then creating the visualizations using this would give more possibilities regarding visualizations.

Regarding the Symphony process itself, the definition of the problem was not defined immediately which led to the initial work being done without a clear guideline. This lack of guidance made the initial work on the report difficult as it was hard to answer: “what should I do?”. This became clear once the problem statement was finalized which in another architectural reconstruction would be the initial focus.

#### Limitations And Future Work

Overall the 2 next steps would be to look into dynamic analysis and try to mitigate some of the shortcomings of solely using skott.

The current approach for architectural reconstruction relies heavily on static analysis, which is not in any way bad, but a combination of dynamic- and static analysis would be preferable. Dynamic analysis compensates for many of the drawbacks of static analysis such as, we can’t detect dead code, we don’t know anything about performance, etc.

Skott is meant for analyzing a single repository and not a monolith repository like the Supabase repository, which in turn means that it cannot capture every reference, take the `apps/studio/package.json` that references the `packages/ui/` module in its `package.json` file. This reference is not shown in the data generated from skott and is therefore hidden.

This limitation of the data skott generates also leaves some manual work when using the tool, to check which projects import each others. While this could be automated and added to the graph, there is also a time constraint on the reconstruction which needs to be considered.

Likewise, the deployment view also contains some manual work that could be automated. One example would be to add ports to the deployment view, which are present in the docker-compose file.

While there are still more limitations to mention, such as the manual way of applying filters to the module view, all of these limitations of the reconstruction are obvious candidates for future work.



## 5. Bibliography

- Antoine-Coulon. (2024). _GitHub - antoine-coulon/skott: All-in-one devtool to automatically analyze, search and visualize dependencies from JavaScript, TypeScript (JSX/TSX) and Node.js (ES6, CommonJS)_. GitHub. [https://github.com/antoine-coulon/skott](https://github.com/antoine-coulon/skott).
- Skonik. (2023). _GitHub - skonik/docker-compose-diagram: 🐳docker-compose + 🎨diagrams = docker-compose-diagram 🐳🎨_. GitHub. [https://github.com/skonik/docker-compose-diagram](https://github.com/skonik/docker-compose-diagram).
- Supabase. (2024). _GitHub - supabase/supabase: The open source Firebase alternative._ GitHub. https://github.com/supabase/supabase
- _Supabase | the open source Firebase alternative_. (n.d.). Supabase. Retrieved May 30, 2024, from [https://supabase.com/](https://supabase.com/).
- _Tutorial — pyvis 0.1.3.1 documentation_. (2023). [https://pyvis.readthedocs.io/en/latest/tutorial.html#filtering-and-highlighting-the-nodes](https://pyvis.readthedocs.io/en/latest/tutorial.html#filtering-and-highlighting-the-nodes).
- Van Deursen, A., Hofmeister, C., Koschke, R., Moonen, L., & Riva, C. (2004). Symphony: view-driven software architecture reconstruction. _Proceedings. Fourth Working IEEE/IFIP Conference on Software Architecture (WICSA 2004)_. https://doi.org/10.1109/wicsa.2004.1310696

## 6. Appendix

The source code of the custom tool have not been uploaded yet, and will be inserted here for the final exam submission