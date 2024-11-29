# How to write good documentation

It's important that documentation is created in the right places according to its intended purpose and target audience.
I found [this documentation system](https://docs.divio.com/documentation-system/) which splits documentation into
tutorials, how-to guides, explanations, and reference.

The system with the 4 documentation types can be retro-fitted to existing documentation technology and structure. It
just helps make a distinction between kinds of documentation, for example when how-to guides are mixed with explanations
which I've seen a lot. I doesn't mean that you have to restructure existing documentation.

## How I interpret the 4 types of documentation

- **Tutorials** are step-by-step guides to help users learn a new skill or tool without a specific application. No
  prior knowledge is assumed. We usually do assume our colleagues to be knowledgeable/for them to follow tutorials by
  themselves if needed. Example: "How do for-loops work in Python?"
- **How-to guides** help users solve a specific problem or achieve a specific goal. Prior knowledge is assumed. Example:
  "How to create secrets for your services on our cloud?"
- **Explanations** are in-depth explanations, discussions how & why a system was set up in a certain way. Not strictly
  necessary to know for users of our systems (i.e. developers), but helpful for context. Example: "How does Vault work
  on our cloud?, "Why do we use Kubernetes distro XYZ for our Kubernetes clusters?"
- **References** are code-determined technical descriptions of a system, e.g. API documentation, configuration options
  of a helm chart. Example: "What are the available options for values.yaml of our shared Vault chart?"

## Additional guidelines that I find useful

- Non-explanations _may_ link to each other and _must_ link to explanations serving as a single source of truth how a
  system works
- Contents of non-explanations _may_ repeat/summarize parts of the explanations
