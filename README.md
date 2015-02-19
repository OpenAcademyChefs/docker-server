# docker-server-cookbook

This cookbook is for testing the functionality of the bflad/chef-docker cookbook on a manged node. I have been reading through the docs of that cookbook, but it has not yet been enough to really grok the workflow. One of the main issues facing docker (and this is only exacerbated when trying to couple docker and chef) is that the workflow is confusing at worst and awkward at best. So this "application" cookbook (intended for deployment to a node) is for my hands-on experimentation with the chef-docker "library" cookbook to find workflow pain points that I can work to ameliorate.

## Supported Platforms

Currently being developed just for Ubuntu 14.04

## Attributes

TODO

<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['docker-server']['bacon']</tt></td>
    <td>Boolean</td>
    <td>whether to include bacon</td>
    <td><tt>true</tt></td>
  </tr>
</table>

## Usage

### docker-server::default

Include `docker-server` in your node's `run_list`:

```json
{
  "run_list": [
    "recipe[docker-server::default]"
  ]
}
```

## License and Authors

Author:: Ryan Chipman (rchipman@mit.edu)
