Sublime Text
============

Ansible role to install sublime, package control and sublime plugins on CentOS or Ubuntu

Requirements
------------

No requirements.

Role Variables
--------------

Set the Sublime-Text version via the `sublime_version` property. Can be one of `"2", "3"`.

    sublime_version: 3

Enable package control via the `sublime_package_control` property.

    sublime_package_control: true

Configure sublime plugins that will be installed via `git` using the `sublime_packages` property. Use the format `[{pluginName: pluginGithiubLink}, ..]`.

    sublime_packages:
      'AdvancedNewFile': 'https://github.com/skuroda/Sublime-AdvancedNewFile.git'
      'Ansible': 'https://github.com/clifford-github/sublime-ansible.git'
      'ColorPicker': 'https://github.com/weslly/ColorPicker.git'
      'Git': 'https://github.com/kemayo/sublime-text-git.git'
      'GitGutter': 'https://github.com/jisaacks/GitGutter.git'
      'Jinja2': 'https://github.com/mitsuhiko/jinja2-tmbundle'
      'Mardown Preview': 'https://github.com/revolunet/sublimetext-markdown-preview'
      'SublimeLinter': 'https://github.com/SublimeLinter/SublimeLinter3.git'
      'Terminal': 'https://github.com/wbond/sublime_terminal.git'
      'TypeScript': 'https://github.com/Microsoft/TypeScript-Sublime-Plugin.git'

Dependencies
------------

No dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: chaosmail.sublime-text }

License
-------

MIT

Author Information
------------------

Christoph Koerner
