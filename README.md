Slightly modified version of original EventManager:

1. Renamed to HubEvent to avoid conflicts
1. Removed promises in favor of callbacks for legacy project support.
2. Repacked functions into object methods for mixing as `Object.assign(this, HubEvents)`.


Previous readme:

```
EventBus.subscribe('useradded', function(user) {
  console.log(user)
});

form.onsubmit(function(e) {
  e.preventDefault();

  // do something with user fields

  EventBus.publish('useradded', user);
})
```
