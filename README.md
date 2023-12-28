import random

def simple_chatbot():
    print("Hello! I'm your AI assistant. You can start a conversation or type 'bye' to exit.")

    while True:
        user_input = input("You: ")
        user_input = user_input.lower()

        if user_input == 'bye':
            print("Goodbye! Have a great day.")
            break
        elif 'how are you' in user_input:
            print("I'm just a computer program, but I'm doing well. Thanks for asking!")
        elif 'name' in user_input:
            print("I don't have a personal name. You can call me ChatBot.")
        elif 'favorite color' in user_input:
            colors = ['red', 'blue', 'green', 'yellow', 'purple']
            print(f"My favorite color is {random.choice(colors)}.")
        else:
            print("I'm sorry, I didn't understand that. Can you ask me something else?")

if __name__ == "__main__":
    simple_chatbot()

