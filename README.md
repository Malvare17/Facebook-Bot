# Facebook-Bot

## About Project
- The program available above uses the powerful and efficient `fb chat` library, which allows us to interact with facebook messenger, using the account login and password.

- The program was created to write messages to people when the account owner is offline or not available

## Installation

- If you use linux make sure you installed `git`, if not write `$ sudo apt install git` in your terminal.

- Install `fbchat` with commend `$ pip install fbchat`.

- At the bottom of the code, enter your password and login in the space provided. Remember to save file.

- Just copy the computer file and run it with the `$ python3 FacebookBot.py` or `$ python FacebookBot.py` command.

### Clone

- Clone this repo to your local machine using `$ git clone https://github.com/Malvare17/Facebook-Bot`

Remember that you run the script at your own risk. Also remember that the program was created for educational purposes and the author is not obliged to do anything.

---
## More options
- If you want, you can add an automatic reply to specific messages.
```python
#Example Code
MessageReceived = message_object.text.lower()

if MessageReceived == "MESSAGE":                
  self.send(Facebook.Message(text="REPLAY")), thread_id = thread_id, thread_type = thread_type)
                self.markAsDelivered(author_id, thread_id)
                self.markAsRead(thread_id)
```
- If you want the program to check if a message belongs to one of many messages and then draw a reply.
```python
#Example Code

#REMEMBER TO IMPORT RANDOM !!!
import random

MessageReceived = message_object.text.lower()

List = ["MESSAGE1", "MESSAGE2"]
List2 = ["MESSAGE3", "MESSAGE4"]

if MessageReceived in List:                
  self.send(Facebook.Message(text=random.choice(List2)), thread_id = thread_id, thread_type = thread_type)
                self.markAsDelivered(author_id, thread_id)
                self.markAsRead(thread_id)
```
