# polymer-tile

A tile component using [Polymer](http://www.polymer-project.org/).

## Demo

[Check it live!](http://teaegg.github.io/polymer-tile-window)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install git://github.com/teaegg/polymer-tile-window.git --save
```

Or [download as ZIP](https://github.com/teaegg/polymer-tile-window/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    ```

2. Import polymer-tile-window:

    ```html
    <link rel="import" href="bower_components/polymer-tile-window/polymer-tile-window.html">
    ```

3. Start using it!

    ```html
    <polymer-tile-window fit>
      <polymer-tile> 
        <tile>
          <tile style="background: yellow;"></tile>
          <tile style="background: red;" linkto="popup2"></tile>
        </tile>
        <tile style="background: orange;" linkto="popup1"></tile>
        <tile double style="background: purple;"></tile>
      </polymer-tile>
      <window id="popup1" fit style="background: orange;">
        <button closeButton>close</button>
      </window>
      <window id="popup2" fit style="background: red;">
        <button closeButton>close</button>
      </window>
    </polymer-tile-window>
    ```

## Options

Method    | Params                   | return             | Description
---       | ---                      | ---                | ---
`restore` | none                     | none               | Navigate to the startup page.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

[MIT License](https://github.com/teaegg/polymer-tile-window/blob/master/LICENSE)
