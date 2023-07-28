# Ablaevent

This library provides an HTTP client for Ablaevent.

## Installation

The package can be installed by adding `elixir` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {ablaevent, "~> 0.1"}
  ]
end
```

## Configuration

```elixir
config :posthog,
  api_url: "http://posthog.example.com",
  api_key: "..."
```

Optionally, you can pass in a `:json_library` key. The default JSON parser is Jason.

## Usage

Capturing events:

```elixir
Posthog.capture("login", distinct_id: user.id)
```

Capturing multiple events:

```elixir
Posthog.batch([{"login", [distinct_id: user.id], nil}])
```
