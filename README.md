# Go Slackbot Age Calculator

This repository contains a Go-based Slackbot that calculates a person's age based on their date of birth. The Slackbot responds to commands in a Slack workspace and provides the calculated age.

## Prerequisites

Before running the Slackbot, make sure you have the following prerequisites installed:

- Go programming language (version 1.16+): [Install Go](https://golang.org/doc/install)
- Slack account: [Create a Slack workspace](https://slack.com/get-started)

## Setup

To set up and run the Slackbot, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/Coffeedragon96/07-go-slackbot-age-calculator.git
   ```

2. Navigate to the project directory:

   ```bash
   cd 07-go-slackbot-age-calculator
   ```

3. Install the project dependencies:

   ```bash
   go mod download
   ```

4. Create a Slack app and bot user in your Slack workspace. Obtain the bot token.

   - Visit the [Slack API website](https://api.slack.com/apps) and create a new app.
   - Enable the "Bots" feature and add a new bot user to your app.
   - Install the app to your workspace.
   - Copy the bot token provided by Slack.

5. Create a `.env` file in the project directory and add the following content:

   ```
   SLACK_BOT_TOKEN=<your-bot-token>
   ```

   Replace `<your-bot-token>` with the bot token obtained from Slack.

6. Run the Slackbot:

   ```bash
   go run main.go
   ```

   The Slackbot will start and connect to your Slack workspace using the provided bot token.

## Usage

Once the Slackbot is running and connected to your Slack workspace, you can interact with it using the following command:

```
/agecalc <date-of-birth>
```

Replace `<date-of-birth>` with the person's date of birth in the format "YYYY-MM-DD". For example: `/agecalc 1990-05-15`.

The Slackbot will respond with the calculated age based on the provided date of birth.

## Contributing

Contributions to this repository are welcome. If you find a bug or have suggestions for improvements, feel free to open an issue or submit a pull request.

Please follow the existing coding style and provide clear commit messages when contributing.

## License

This repository is licensed under the [MIT License](LICENSE). Feel free to use and modify the code according to the terms of the license.

## Acknowledgments

This Slackbot project was inspired by the need to quickly calculate ages in Slack conversations. Special thanks to the Slack API documentation and the Go community for providing the necessary tools and resources to build this project.
