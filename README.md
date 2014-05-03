genymotion Cookbook
===================
Installs Genymotion
TODO: Finish the _debian recipe, it grabs geny, but doesnt run the installer.bin


Requirements
------------
#### packages
- `java` - of course

Attributes
----------
none at this time, you get version 2.22

Usage
-----
The way I install genymotion is by setting cookbooks/android-studio/attributes/default.rb:
`default[:android][:emulator][:genymotion] = true`

But you could just add it to a run_list
Just include `genymotion` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[genymotion]"
  ]
}
```

Contributing
------------
TODO: (optional) If this is a public cookbook, detail the process for contributing. If this is a private cookbook, remove this section.

e.g.
1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write your change
4. Write tests for your change (if applicable)
5. Run the tests, ensuring they all pass
6. Submit a Pull Request using Github

License and Authors
-------------------
Authors: TODO: List authors
