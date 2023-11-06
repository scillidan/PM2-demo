## Localhost

```sh
cd client
yarn install
yarn build
mv build ../server/
```

```sh
cd ../server
python310 -m venv venv
venv\Scripts\activate.bat
pip install -r requirements.txt
python server.py
```

Open `localhost:2628`, then add `dictionnary-file` into `source/`.

Some cache saved on `C:\Users\yourname\.silverdict` and `C:\Users\scillidan\.cache\SilverDict`.