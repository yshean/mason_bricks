<p align="center">
<a href="https://pub.dev/packages/mason"><img src="https://raw.githubusercontent.com/felangel/mason/master/assets/mason_full.png" height="125" alt="mason logo" /></a>
</p>

<p align="center">
<a href="https://github.com/felangel/mason/actions"><img src="https://github.com/felangel/mason/workflows/mason/badge.svg" alt="mason"></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-purple.svg" alt="License: MIT"></a>
</p>

<p align="center">
A collection of bricks that helps developers to generate files with a Dart template generator called [Mason](https://pub.dev/packages/mason).
</p>

---

Interested in creating your own brick? Here's how I created my first brick (`model_freezed_json`):

1. Install `mason_cli` with `dart pub global activate mason_cli`
2. Create a directory called `bricks`
3. In the directory, run `mason init`
4. Create a brick with `mason new model_freezed_json --desc "Generate a model that uses freezed and json_serializable"`
5. Install my own brick `mason add model_freezed_json --path .\model_freezed_json\` so I can test locally before publishing to the registry
6. Edit the files in `__brick__` -- these are the files that will be generated when you run your brick (`mason make model_freezed_json --name person -o ./models`)
7. When it's good enough, publish to your own GitHub and then [BrickHub.dev](https://brickhub.dev/) with `mason publish` 🚀