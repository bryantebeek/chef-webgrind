Webgrind Cookbook
====================
Allows for installation of Webgrind on Debian (/Ubuntu) boxes.

Requirements
------------

#### packages
- `php` - Webgrind runs using PHP.
- `apache2` - Webgrind uses apache2 to display the front-end.

Attributes
----------
<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['webgrind']['docroot']</tt></td>
    <td>String</td>
    <td>The document root where webgrind is going to be installed</td>
    <td><tt>/var/www/webgrind</tt></td>
  </tr>
  <tr>
    <td><tt>['webgrind']['access_url']</tt></td>
    <td>String</td>
    <td>The url to access webgrind (default: mywebsite.app**/webgrind**)</td>
    <td><tt>/webgrind</tt></td>
  </tr>
</table>

Usage
-----
Just include `webgrind` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[webgrind]"
  ]
}
```

Contributing
------------

1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write you change
4. Write tests for your change (if applicable)
5. Run the tests, ensuring they all pass
6. Submit a Pull Request using Github

License and Authors
-------------------
Authors: Bryan te Beek
