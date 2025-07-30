### Octra Public Testnet

#### Join Discord
https://discord.gg/octra

#### System Requirements (Use any of the listed systems)
- Linux Ubuntu OS
- VPS: You can use a linux VPS to follow the guide
- Windows: Install Linux Ubuntu using WSL by following this guide
- Codespace: If you don't have VPS or Windows WSL, you can use Github Codespace, create a blank template and run your codes.

Use [Moei's Guide](https://github.com/0xmoei/octra) to setup the CLI (Task 2) where we transact with other octra addresses using encrypt and decrypt functions for private transactions.

Make sure to update the CLI in Task 2. Run the below command if you haven't already.
```
cd octra_pre_client
git pull origin main
```
`If you see an error about uncommitted changes (e.g., in cli.py or other files), stash your changes:`
```
git stash
git pull origin main
```

<img width="400" height="100" alt="Screenshot 2025-07-30 100639" src="https://github.com/user-attachments/assets/bb8789a1-1b37-4aca-92a7-19117d53dc42" />

`If you get this image at any point of updating, you have done it well, no need to repeat.`

You can also interact with my wallet `octAv8GZbQCcYr2k8WkJ2kABv4kQirFRuXBDc7UCdR8hUtKt`, send some tokens while encrypted and not, I will send back.

Install requirements:
```
python3 -m venv venv

source venv/bin/activate
pip install -r requirements.txt
```
---

> If you are using the same terminal from the update to do task 3 do this.

```
deactivate
```
Now run this to leave any previous directories you were inside
```
cd ~
```
---

### Task 3
Install Rust if you don't already have it.
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```
You will be prompted to proceed, just hit `Enter` to use default installation.

#### Build `ocs01-test` from Source
Build from source
```
git clone https://github.com/octra-labs/ocs01-test.git
cd ocs01-test
cargo build --release
```
> Once it is done, you will get a `Finished` line and the line where you can paste commands returns so you can continue with the guide.

### Setup the files to test
Copy the Contract interface
```
cp EI/exec_interface.json .
```

Copy your wallet.json file from `Task 2` into the `ocs01-test` folder
```
cp ~/octra_pre_client/wallet.json ~/ocs01-test/
```

Copy the binary from `target` folder in `ocs01-test` to the `ocs01-test` main directory.
```
cp ~/ocs01-test/target/release/ocs01-test ~/ocs01-test/
```

`NB`: `These three (3) files must be in the same directory (~/ocs01-test/) for them to work together.

Confirm using the command `ls -l` or `ls -a` while in the /ocs01-test/.
If you are not sure you are in the folder run this command `cd && cd ocs01-test then run `ls -l` or `ls -a`.

Now that you are sure all three (3) files are in the same folder, let's start testing task 3.
While still in `/ocs01-test/` folder or directory, run this `start` command
```
./ocs01-test
```
You should get the below interface.

<img width="400" height="300" alt="Screenshot 2025-07-30 102219" src="https://github.com/user-attachments/assets/0faa4e11-2d94-4b7c-99a9-fba0c1fcddd5" />

If it fails and gives you this error below, just rerun the `start` command again, it would come up.

<img width="300" height="100" alt="Screenshot 2025-07-30 102559" src="https://github.com/user-attachments/assets/9b242354-371c-4e6c-a505-4ba53f13c4ed" />

If yours has worked, now get testing 🔥🔥🔥
`choice`: `3` and enter. Your screen should look like this.

<img width="400" height="130" alt="Screenshot 2025-07-30 103009" src="https://github.com/user-attachments/assets/6db8b402-c033-408d-982b-6a4c3ccc18a1" />

This task `3` helps you to secure the reward or main quest of this test phase. `3` gives you the 1 test token allocated once to any address that does this task.

Now you can randomly make any other `choice` from the list between `0-14` including `3`. Run as much as you can and welcome to the future of FHEs.
gOctra! 🎉

Contact me on X if you get any other errors. [dee 宫](https://x.com/dee__analyst)
