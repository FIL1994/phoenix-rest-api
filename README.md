# MyApp

## Create App
```sh
mix phx.new my-app --app my_app --module MyApp --no-html --no-webpack
```

## Generate User Schema and Auth Context Modules
```sh
mix phx.gen.context Auth User users email:string:unique \is_active:boolean
mix ecto.migrate
```
Help
```sh
mix help phx.gen.context
```

## Generate a New JSON Endpoint
```sh
mix phx.gen.json Auth User users email:string password:string is_active:boolean --no-context --no-schema
```

To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Start Phoenix endpoint with `mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix
