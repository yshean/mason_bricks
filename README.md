Welcome to my bricks! 👋

Here's how I created my first brick (`model_freezed_json`):
1. Install mason_cli with `dart pub global activate mason_cli`
2. Create a directory called `bricks`
3. In the directory, run `mason init`
4. Create a brick with `mason new model_freezed_json --desc "Generate a model that uses freezed and json_serializable"`
5. Install my own brick `mason add model_freezed_json --path .\model_freezed_json\` so I can test locally before publishing to the registry
6. Edit the files in `__brick__` -- these are the files that will be generated when you run your brick (`mason make model_freezed_json --name person -o ./models`)
7. When it's good enough, publish to your own GitHub and then [BrickHub.dev](https://brickhub.dev/) with `mason publish` 🚀