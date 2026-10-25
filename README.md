🚀 Projector

A smarter way to create projects from reusable templates.

"Python" (https://img.shields.io/badge/Python-Automation-blue?logo=python&logoColor=white)
"Automation" (https://img.shields.io/badge/Automation-Enabled-00C853)
"Templates" (https://img.shields.io/badge/Reusable-Templates-purple)

«Build faster. Reuse smarter. Create more.»

Projector is a Python-based project generator that automates project creation using reusable templates. Generate new projects without manually copying folders, renaming files, or replacing project-specific text.

✨ Features

- ⚡ Automated project generation
- 🧩 Reusable project templates
- 🔄 Automatic placeholder replacement
- ⚙️ JSON-based configuration
- 📁 Automatic file and directory copying
- 🛠️ Customizable project generators
- 📦 Binary file contents skipped during text replacement

📑 Table of Contents

- "Installation" (#-installation)
- "Quick Start" (#-quick-start)
- "Available Generators" (#-available-generators)
- "How It Works" (#-how-it-works)
- "Configuration" (#-configuration)
- "Custom Templates" (#-custom-templates)
- "Template Syntax" (#-template-syntax)

🛠️ Installation

Clone the repository:

git clone https://github.com/palikar/projector.git
cd projector

Install Projector:

python setup.py install

🚀 Quick Start

Create a new CMake project:

projector cmake-simple ~/code/new_project

List available project generators:

projector --list-gen

🧠 How It Works

       PROJECTOR
           |
           v
   Select a template
           |
           v
   Configure properties
           |
           v
     Copy template
           |
           v
 Replace placeholders
           |
           v
   Generate project

Projector copies a selected template, collects property values, and replaces matching placeholders in supported filenames and text files.

⚙️ Configuration

Project generators are defined in "config.json".

Each generator specifies a template directory and a list of properties.

Example property configuration:

{
  "name": "Project name",
  "token": "project_name",
  "default": "MyProject"
}

Configuration fields

Field| Description
"root_dir"| Template directory
"properties"| List of project properties
"name"| User prompt
"token"| Placeholder identifier
"default"| Optional default value

🎨 Custom Templates

Create your own templates:

1. Create a template directory.
2. Add your starter files.
3. Insert placeholders into supported filenames and text files.
4. Add a generator configuration to "config.json".
5. Run Projector using your generator name.

🔤 Template Syntax

Projector's README describes Mustache-style templates.

Example:

Project Name: {{project_name}}
Author: {{author}}

Generated output:

Project Name: MyProject
Author: Developer

Check your installed version's implementation to confirm the supported placeholder syntax.

🔮 Future Improvements

- [ ] More programming language templates
- [ ] Interactive project setup
- [ ] Improved error handling
- [ ] Automated testing
- [ ] Template validation
- [ ] More customization options

📄 License

Check the repository for license information.

---

<p align="center">
  <b>BUILD • AUTOMATE • CREATE</b>
  <br>
  Made for developers who value their time. ⚡
</p>
