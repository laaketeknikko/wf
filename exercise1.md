Language: C++

For linting in C++, a popular tool seems to be clang-tidy.
Clang itself is some sort of a family of tools like analyzing
and compilers. Similar tools are provided by Visual C++ by Microsoft. A popular open source version is GCC.
For testing, again there is Visual C++, or for example GoogleTest.

Perhaps it is only the impression I get, or perhaps it's
because of the focus on the npm ecosystem in the course,
but the offerings for C++ seem quite fragmented. Whereas in
JavaScript it would seem a linter for a library might be
an extension for ESLint, for C++ bigger libraries like Qt
seem to have their own linters.

For example, Qt has its own unit testing and end-to-end testing
library, its own build system, a linter and so on.

For CI work, there seem to be many options, such as GitLab,
Azure DevOps, or more specialized solutions like Felgo
for building cross-platform with the Qt framework.

For deciding between self-hosting and cloud-based, I would
imagine the answer is language-agnostic. For very small projects, The "CI" system might be less than is supported by
any real solution, apart from other manual solutions like CMake.

For very big projects, on the other hand, you would have the resources to self-host. You also might not trust any providers
with your nuclear missile codebase.

CI services are probably the best choice for many projects
between these two, where the project might actually benefit,
but there isn't expertise available to roll your own.
