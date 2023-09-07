
You are assigned to refactor a piece of code to improve its design using the Adapter design pattern. The code you are provided with interacts with a legacy library that has a different interface from the one you desire. Your task is to implement an adapter that allows the code to work seamlessly with the legacy library.

Code:
```
# Existing Code Snippet

class NewLibrary:
    def perform_operation(self, data):
        # Perform operation using the new library
        pass

class ClientCode:
    def __init__(self, library):
        self.library = library

    def execute_operation(self, data):
        self.library.perform_operation(data)

# Usage
new_library = NewLibrary()
client_code = ClientCode(new_library)
client_code.execute_operation("Data to process")
```

Requirements:
1. Identify the design issues in the given code snippet.
2. Apply the Adapter design pattern to refactor the code.
3. Implement the adapter class to bridge the gap between the desired interface and the legacy library.
4. Modify the client code to use the adapter class instead of directly interacting with the legacy library.
5. Provide a detailed explanation of the Adapter design pattern and how it addresses the design issues in the original code.
