Bowtie Integration Example Structure
===

This is a simple repo to outline to structure of your documented integrations.

Creating an integration is easy:

###Step 1: Proof of Concept in Static Website

Make a working example in the src/ directory. Users will clone this entire repo and look at the src code for an example.

### Step 2: Bundle Assets for Use by Others

Extract the integration assets, bundle them for distribution, and move them into your dist/ folder. Any configuration (api keys, etc) need to be extract from the minified bubundle.

---

More Details
---

As we build our first 10 integrations, we want to follow a specific, repeatable guidelines. That being said, we also want to be descriptive in our git commits, code comments, and overall approach to solving problems. This will allow other bowtie users to extend you integrations and contribute online.


### Your src/ directory

Your src/ directory is your demo directory. It's important that your realize most users will run this jekyll build before integrating your code.

* Write a README.md for this file


### Your dist/ directory

Your bundled assets need to follow a few specific guidelines.

* All assets must be minified. These are blind assets anyone can copy into their site without needing to customize.

* Follow this naming structure:
  * integration_name.bundle.min.js && integration_name.bundle.min.css



TODO
---

* Add a single Gulpfile that makes bundling assets consistent and repeatable.


