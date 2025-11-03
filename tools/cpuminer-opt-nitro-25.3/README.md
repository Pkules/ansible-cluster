# cpuminer-opt-nitro

**Nitro Edition** — customized and maintained by [NitroPool](https://nitropool.net),
based on `cpuminer-opt` by JayDDee and other community contributions.

This version includes:

* Custom banners
* NitroPool branding
* Support for small miner communities
* Full algorithm support with low-diff mining focus

---

### 🛠️ Requirements

1. **64-bit CPU** supporting:

   * x86\_64 (Intel/AMD with SSE2)
   * or ARMv8-aarch64 with NEON

2. **64-bit OS**:

   * Linux (tested), BSD, macOS, or Windows

3. **Stratum support**:

   * stratum+tcp\:// or stratum+ssl://
   * Also supports getblocktemplate (Gbt) via http(s)://

---

### ⚙️ Compile Instructions (Linux)

```bash
sudo apt update
sudo apt install git build-essential automake autoconf libcurl4-openssl-dev libjansson-dev libgmp-dev
git clone https://github.com/No-F8/cpuminer-opt-nitro.git
cd cpuminer-opt-nitro
./autogen.sh
./configure
make -j$(nproc)
```

Output binary will be `./cpuminer`.

---

### 📦 Precompiled Binaries

Precompiled binaries for Linux and Windows are available on the [Releases](https://github.com/No-F8/cpuminer-opt-nitro/releases) page.

* 🐿 [Linux x86\_64 Release](https://github.com/No-F8/cpuminer-opt-nitro/releases/latest)
* 🪿 [Windows 64-bit Release](https://github.com/No-F8/cpuminer-opt-nitro/releases/latest)

---

### ⚡ Supported Algorithms

```
allium           anime            argon2          argon2d250
argon2d500       argon2d4096     blake           blake2b
blake2s          blakecoin       bmw             bmw512
c11              decred          deep            dmd-gr
groestl          hex             hmq1725         jha
keccak           keccakc         lbry            lyra2h
lyra2re          lyra2rev2       lyra2rev3       lyra2z
lyra2z330        m7m             minotaur        minotaurx
myr-gr           neoscrypt       nist5           pentablake
phi1612          phi2            polytimos       power2b
quark            qubit           scrypt          scrypt:N
scryptn2         sha256d         sha256dt        sha256q
sha256t          sha3d           sha512256d      skein
skein2           skunk           sonoa           timetravel
timetravel10     tribus          vanilla         veltor
verthash         whirlpool       whirlpoolx      x11
x11evo           x11gost         x12             x13
x13bcd           x13sm3          x14             x15
x16r             x16rv2          x16rt           x16rt-veil
x16s             x17             x20r            x21s
x22i             x25x            xevan           yescrypt
yescryptr8       yescryptr8g     yescryptr16     yescryptr32
yespower         yespowerr16     yespower-b2b    zr5
```

Note: some variants of scrypt/yespower require additional flags like `--param-n`, `--param-r`, and `--param-key`.


### 💬 Support & Bugs

Report issues here:

* GitHub: [https://github.com/No-F8/cpuminer-opt-nitro/issues](https://github.com/No-F8/cpuminer-opt-nitro/issues)
* Discord: [NitroPool Discord](https://discord.gg/YOUR_INVITE)

Always include your full command line and full console output.
[CHANGE TO YOUR WALLET]

```bash
./cpuminer -a yescryptR16 -o stratum+tcp://nitropool.net:6236 -u web1qfgs9zwgrs3e3kxa0sq7elvhwthj5s5e7r94uhq -p c=BTE
```

---

### 🙏 Donations

No dev fee. Donations welcome to support NitroPool development:

* BTC: `bc1qt2zkl0udsu4c0aptc29fcq9xxmmgk0he8kaerp`
* DOGE: `DPfv3By7Fy5n1x23xgAK6edg1mRQ23vf8R`

Happy hashing — from the NitroPool team. 🔧
