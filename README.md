# Tutorial for change the Default Linux Terminal Shell

Here's a clear formulation in English:

### Change the Default Linux Terminal Shell to Fish

1. **Install Fish**:
   First, install the Fish shell with the following command:

   ```bash
   sudo apt install fish
   ```

2. **Check Fish Installation Path**:
   Verify the installation path of Fish by running:

   ```bash
   which fish
   ```

   The output should be something like `/usr/bin/fish`.

3. **Add Fish to Authorized Shells**:
   If Fish is not listed in the authorized shells, you need to add it manually. Use this command to append the Fish path to the `/etc/shells` file:

   ```bash
   echo /usr/bin/fish | sudo tee -a /etc/shells
   ```

4. **Change the Default Shell**:
   Now, change the default shell for your user by running:

   ```bash
   chsh -s /usr/bin/fish
   ```

5. **Start Fish Immediately**:
   To start using Fish immediately without restarting or logging out, type:

   ```bash
   fish
   ```
