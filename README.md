# CodeAlpha_Basic_Chatbot
def basic_chatbot():
    print("Chatbot: Hello! I am a simple rule-based chatbot.")
    print("Chatbot: You can say 'hello', ask 'how are you', or type 'bye' to exit.")
    
    # 1. Main chat loop
    while True:
        user_input = input("\nYou: ").lower().strip()
        if user_input in ["hello", "hi", "hey"]:
            print("Chatbot: Hi there! How can I help you today?")
            
        elif user_input == "how are you" or user_input == "how are you?":
            print("Chatbot: I'm just a few lines of Python code, but I'm doing great! Thanks for asking.")
            
        elif "name" in user_input:
            print("Chatbot: I am the CodeAlpha Basic Chatbot.")
            
        elif user_input in ["bye", "goodbye", "exit", "quit"]:
            print("Chatbot: Goodbye! Have a wonderful day!")
            break # This stops the loop and ends the program
            
        else:
            print("Chatbot: I'm sorry, I don't quite understand that. Try saying 'hello', 'how are you', or 'bye'.")

if __name__ == "__main__":
    basic_chatbot()
