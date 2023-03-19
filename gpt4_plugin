from steamship import Steamship
# Create a Steamship client
# NOTE: When developing a package, just use `self.client`
client = Steamship(workspace="my-unique-name")

# Create an instance of this generator
generator = client.use_plugin('gpt-4')
# Generate text
task = generator.generate(text=input('enter some words:'))

# Wait for completion of the task.
task.wait()

# Print the output
print(task.output.blocks[0].text)
