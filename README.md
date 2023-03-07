# TTT-docs
Documentation for TTT.

## Types of documentation
There are three types of documentation included in this repository:

- HTML
- LaTeX
- man

## Generating the documentation
### Dependencies
To generate the documentation you will need these dependencies:

- git
- doxygen

Generating the documentation requires that you clone the TTT repository as well as the TTT-docs repository.

**Why?**

It's because the TTT repo has the documentation and the Doxyfile needed to generate it and the TTT-docs repository is used to separate the library from the documentation and to not clutter the repository.

### Cloning the repositories
You need to execute this commands:

```bash
$ git clone https://github.com/reallySmooll/TTT.git
$ git clone https://github.com/reallySmooll/TTT-docs.git
```

### Actually generating the docs and moving them to the appropriate directories
To do that, you will need to execute this commands:

```bash
$ cd TTT/
$ doxygen
$ rm -rf ../TTT-docs/docs/
$ mv docs/ ../TTT-docs/
```

And that's it! You now have basically offline TTT documentation.

## Contributing
There are to ways in which you can contribute:

- Making the site look prettier
- Changing the documentation to add more information for example

### Making the site look prettier
The TTT documentation uses a third party project called `Doxygen Awesome`, Which basically makes the site prettier automatically but it also has a ton of customization with which you can help.

The directory `docs/` contains a file called `custom.css` which is used to customize Doxygen Awesome. If you'd like to help, read up on the documentation of Doxygen Awesome and edit the `custom.css` file then commit the changes and make a pull request. I will review it and maybe you'll get your request pulled.

### Changing the documentation
There's not much to it really. Go to any of the TTT library files and look for any comments starting with a `/**` or a `///<`. These are comments that Doxygen uses to generate the documentation. Next, change them to add more information or change the information or remove some information, whatever. Commit your changes, make a pull request and wait.

## Third party projects
[Doxygen Awesome](https://www.github.com/jothepro/doxygen-awesome-css) - jothepro
