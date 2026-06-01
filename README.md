username = input("Create username: ")
password = input("Create password: ")

attempts = 3

while attempts > 0:
    print("\n--- Login ---")

    login_username = input("Username: ")
    login_password = input("Password: ")

    if login_username == username and login_password == password:
        print("Login successful!")
        break
    else:
        attempts -= 1
        print(f"Incorrect! Attempts left: {attempts}")

if attempts == 0:
    print("Account locked!")
    
