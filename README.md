# Outlook Simulator (Python)

This is an Outlook Simulator I built because I wanted to know how email systems truly worked behind the scenes. Instead of doing some generic project, I wanted to develop something that felt like an achievement and actually let me practice building a system rather than a single script.

It runs in the command-line, generates a mailbox, and allows you to interact with emails the way you would in a simplified version of Outlook. I also added some custom email types, a basic encryption feature, and some little analytics for personal messages.

---

## What This Project Does

- Creates a fake mailbox that's filled with generated emails
- Lets you interact with the mailbox through a simple command-line prompt
- Supports several types of emails:
  - **Normal Mail**
  - **Confidential Mail** (hidden body and custom encryption)
  - **Personal Mail** (extra stats like a word count)

- This project lets you:
  - List emails
  - Open an email
  - Filter by sender
  - Search by date
  - Mark emails as flagged or read
  - Move emails to different tags
  - Soft-delete emails (moving them to the "bin")
  - Add your own emails directly through the command-line interface

A tiny, text-based outlook I built all from scratch.

---

## Why I Built It

I wanted a proper project that showcases I can:
- Work with several Python files and classes
- Build something that feels like a proper application
- Parse data and turn it into structured objects
- Design a system with different components talking to each other
- Add my own ideas like encryption and analysis

This project essentially helped me fully understand how email clients organise data, how command interpreters work, and how to design a program that's easy to extend/ modify later.

---

## How It's Structured

I kept the structure simple, making it easier to follow:
```
Outlook_Simulator/
│
├─ Mail.py             # Base email class
├─ Confidential.py     # Confidential email type (hidden body and custom encryption)
├─ Personal.py         # Personal email type (analytics)
├─ MailboxAgent.py     # Mailbox controller (searching, tagging, and parsing)
└─ Interpreter.py      # Command-line interface
```

Each file has its own job, and with all of them the simulator will run!

---

##  How To Use It

1. Clone the repo
2. Open it in your IDE (I used PyCharm)
3. Run ```Interpreter.py```
4. You'll get a prompt like this:
```
mba>
```

After that, you can use commands like:
```
lst                    # List all the emails
get 3                  # Open email with ID 3
flt email5@gre.ac.uk   # Filter emails by sender
fnd 12/5/2025          # Find emails by date
add sender receiver date subject tag %% message body here
del 7                  # Delete email with ID 7
mrkr 4                 # Mark email with ID 4 as read
mv 2 work              # Move email with ID 2 with "work" tag
end                    # Exit the simulator
```

Just gives you a quick feel for how the Mailbox system works.

---

## Things I Might Add Later

- A small GUI (PyQT or Tkinter)
- Further developed encryption
- Reply/ forward functionality
- Logging or exporting emails
- Saving the mailbox data between sessions

I could definitely expand this project, but it was built at the current learning level I was ongoing.

---

## Final Thoughts

Overall, this project was genuinely really fun to build and definitely helped me comprehend how email clients work behind the scenes. If you're a developer or recruiter checking out my work, thanks for taking your time to observe my program. If you have any feedback, improvement ideas, and internship opportunities, I'm always open to being even greater.
