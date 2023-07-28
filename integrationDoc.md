# Setup Elixir

Follow the instructions below to send custom events from your Elixir backend.

## Install

````
def deps do
    [
        {:ablaevent, "~> 0.1"}
    ]
end

````
## Configure

````
config :posthog,
    api_url: "https://e.abla.io",
    api_key: "PHC"

````
