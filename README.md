# ansible-collection-gitea

## Development

Currently, all roles (inside roles/) are Git submodules, and work on the roles themselves
should take place in the upstream Role repository.

Adding a role (submodule)

```
cd roles
git submodule add https://github.com/dev/repo
```

Updating all roles (submodules)

```
git submodule update --recursive --remote
```

After updating roles, commit and push all changes, and make sure the collection works as expected.
Then tag the new version of the collection and push the tag.