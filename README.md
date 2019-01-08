how to compile the enaqfa GUI wallet?
...



**1. Clone wallet sources**

```
git clone https://github.com/enaqfa/enaqfa-wallet.git
```

**2. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../enaqfa cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/enaqfa/enaqfa-core.git cryptonote
```

Replace URL with git remote repository of your coin.

**3. Build**

```
mkdir build && cd build && cmake .. && make
```
