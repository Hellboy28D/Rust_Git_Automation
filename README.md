# Rust_Git_Automation

🚀 Rust Git Automation

A lightweight command-line utility written in Rust that automates the most common Git workflow:

Stage → Commit → Push

Instead of typing multiple Git commands every time you make changes, this application performs the entire process with a single execution while generating a unique commit message automatically.

⸻

📖 Overview

Rust Git Automation is a CLI tool that simplifies everyday version control tasks.

Whenever you run the program, it automatically:

1. Stages every modified, deleted, and newly created file.
2. Generates a random commit message.
3. Creates a Git commit.
4. Pushes the changes to the configured remote repository.

This project demonstrates how Rust can interact with external system processes using std::process::Command while maintaining excellent performance and reliability.

⸻

✨ Features

* ⚡ One-command Git workflow
* 📂 Automatically stages all repository changes
* 🎲 Generates random commit messages
* 💻 Executes native Git commands from Rust
* 🚀 Pushes directly to the remote repository
* 🦀 Written entirely in safe Rust
* 📦 Lightweight and fast
* 🔧 Easy to customize

⸻

🛠 Technologies Used

* Rust
* Cargo
* std::process::Command
* names crate
* Git

⸻

📁 Project Structure

Rust_Git_Automation/
│
├── src/
│   └── main.rs
│
├── Cargo.toml
├── Cargo.lock
├── README.md
└── .gitignore

⸻

⚙️ How It Works

The application performs three Git operations sequentially.

Step 1

Stage every file inside the repository.

git add -A

⸻

Step 2

Generate a random commit message.

Example:

happy-lion
silent-dragon
blue-falcon
fancy-tiger

Then execute:

git commit -m "<generated-name>"

⸻

Step 3

Push the latest commit.

git push origin master

If every command succeeds, the program prints:

Successfully added, committed, and pushed changes!

⸻

🚀 Installation

Clone the repository.

git clone https://github.com/Hellboy28D/Rust_Git_Automation.git

Move into the project.

cd Rust_Git_Automation

Install dependencies.

cargo build

Run the application.

cargo run

⸻

📦 Dependencies

[dependencies]
names = "*"

⸻

🧠 Code Highlights

The project demonstrates several useful Rust concepts.

* Executing external programs
* Error handling
* Process management
* Command-line automation
* Ownership and borrowing
* Modular function design
* Returning String
* Working with third-party crates

⸻

📌 Example Workflow

Suppose you edited several files.

Instead of running:

git add -A
git commit -m "Updated project"
git push origin master

Simply execute:

cargo run

The program handles the rest automatically.

⸻

📈 Future Improvements

This project can be extended with many useful features.

* Support main and master branch detection
* Automatic branch discovery
* Custom commit message templates
* Interactive CLI
* Colored terminal output
* Logging
* Git status preview
* Dry-run mode
* Push to multiple remotes
* GitHub API integration
* Semantic version tagging
* Commit history analytics
* Cross-platform installer
* Configuration file support
* Scheduled automatic commits

⸻

⚠️ Current Limitation

The current implementation assumes the default branch is:

master

If your repository uses:

main

Change:

.arg("master")

to

.arg("main")

or improve the project by detecting the current branch automatically.

⸻

🎯 Learning Outcomes

Building this project helps understand:

* Rust process management
* Executing shell commands safely
* CLI application development
* Error propagation
* Git automation
* Systems programming with Rust
* Using external crates
* Writing maintainable Rust code

⸻

🤝 Contributing

Contributions are welcome.

You can contribute by:

* Improving error handling
* Adding more Git commands
* Supporting configuration files
* Implementing automatic branch detection
* Enhancing the CLI interface
* Writing unit tests
* Improving documentation

Feel free to fork the repository, open issues, or submit pull requests.

⸻

📜 License

This project is available under the MIT License.

⸻

⭐ Support

If you found this project useful or learned something from it, consider giving the repository a ⭐ on GitHub.

Your support helps the project grow and motivates further development.

⸻

👨‍💻 Author

Hellboy28D

Building high-performance Rust applications, developer tools, AI systems, and open-source projects one repository at a time.
