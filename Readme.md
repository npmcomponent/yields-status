*This repository is a mirror of the [component](http://component.io) module [yields/status](http://github.com/yields/status). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-status`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# status

  User &quot;active&quot; / &quot;idle&quot; event emitter.

## Example

```js
var status = requrie('status');
status.watch();

status('idle', function(){
  console.log('idle!');
});

status('active', function(){
  console.log('active!');
});
```

## Installation

    $ component install yields/status

## API

### status.watch([timeout])

Start watching on `mousemove` and `keyup` the default `timeout` is 1 minute.

### status.unwatch()

Stop watching `mousemove` and `keyup`.

### status(event, fn)

Invoke `fn` on `event`.

## Todo

  * add tests.

## License

  MIT
