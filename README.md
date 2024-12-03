# VOOI - TELEGRAM BOT

This script will automate the vooi api in the telegram miniapp, performing tasks properly in the miniapp for example: completing tasks, running the autotrade function and also opening or closing trade positions.

[TELEGRAM CHANNEL](https://t.me/airdropconfirm97) | [CONTACT](https://t.me/airdropconfirm97)

### Please support me by buying me a coffee: 
```

```

## REGISTER VOOI AIRDROP

 Vooi powered by chain abstraction | Backed by BinanceLabs, accelerated by Consensys & ZK Accelerator.
 
 1. Start [t.me/VooiAppBot](https://t.me/VooiAppBot/vooi?startapp=frenIDGBXq0XL)
 2. Open the Apps 
 3. Start "Auto Trade"
 4. Play Taps Taps Game
 5. Complete Available Quest

## Features
- Completing All Available Quest
- Run the Autotrade Function
- Auto Open and Close Trade Position `Configurable`
- Auto Play Taps Game `Configurable`
- Multi Account Support 
- Proxy support for multiple accounts.
- Configurable through `config.json`.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/CRYPTOMASTER09/Vooi-bot.git
   cd Vooi-bot
      ```
2. **Create a virtual environment (optional but recommended)**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Dependencies:**

The bot uses Python 3 and requires some external libraries. You can install them using:

  ```bash
    pip install -r requirements.txt
  ```

### Dependencies include:

   ```txt
cloudscraper==1.2.60
colorama==0.4.6
python-dateutil==2.8.2
pytz==2023.3
   ```

## Configuration Setup:

Create a `config.json` file in the project root directory:

   ```json
 {
     "use_proxy": false,
     "open_position": false,
     "auto_complete_task": false,
     "auto_play_game": false,
     "profit_threshold": 0.4,
     "loss_threshold": -0.9,
     "max_game_to_play": 6,
     "account_delay": 5,
     "countdown_loop": 1000
 }
   ```
- `use_proxy`: Enable/disable proxy usage (true/false).
- `open_position`: Enable/disable auto open position fuction (true/false).
- `auto_complete_task`: Enable/disable auto complete quest (true/false).
- `auto_play_game`: Enable/disable auto play taps game (true/false).
- `profit_threshold` and `loss_threshold`: Min and max profit or loss to close position in % x10
- `max_game_to_play`: Number of the taps game to play `default 6`
- `account_delay`: Delay (in seconds) between processing each account.
- `countdown_loop`: Time (in seconds) before restarting the bot cycle.

## Query Setup:

Add your VOOI account tokens to a file named `data.txt` in the root directory. Each token should be on a new line.

1. Use PC/Laptop or Use USB Debugging Phone
2. open the `VOOI telegram bot`
3. Inspect Element `(F12)` on the keyboard
4. at the top of the choose "`Application`" 
5. then select "`Session Storage`" 
6. Select the links of "`VOOI`" and "`tgWebAppData`"
7. Take the value part of "`tgWebAppData`"
8. take the part that looks like this: 

```txt 
user=xxxxxxxxx-Rxxxxxxx&hash=xxxxxxxxxxx
```
9. add it to `data.txt` file or create it if you dont have one


You can add more and run the accounts in turn by entering a query id in new line like this:
```txt
query_id=xxxxxxxxx-Rxxxxxxx&hash=xxxxxxxxxxx
user=xxxxxxxxx-Rxxxxxxx&hash=xxxxxxxxxxx
```

### Proxy Setup (Optional):

If you enable proxy support in `config.json`, create a `proxies.txt` file in the root directory, containing a list of proxies, one per line.

Example (proxy format: username:password@host:port):

   ```graphql
http://user1:pass1@123.123.123.123:8080
socks5://user2:pass2@456.456.456.456:8080
   ```

## Usage
Run the script with:

   ```bash
python main.py
   ```

***The bot will:***

Load the accounts from `data.txt`.
Process each account by fetching user info, performing daily sign-in, opening all boxes, executing quacks, and completing tasks (if enabled).

## License
This project is licensed under the `MIT License`.

## Contact
For questions or support, please contact [ https://t.me/airdropconfirm97 ]