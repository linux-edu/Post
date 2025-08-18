🖥️ Linux System Management Essentials

6 commands to master your machine!

1️⃣ uname -a

🔹 What it does: Shows your Linux kernel + system details.
💻 Try it:

```bash
uname -a
```

📌 Example output:

```bash
Linux mypc 5.15.0-76-generic #83-Ubuntu SMP x86_64 GNU/Linux
```

💡 Pro Tip: Use just uname -r for kernel version only!

---

2️⃣ df -h

🔹 What it does: Checks disk space (human-readable format).
💻 Try it:

```bash
df -h
```

📌 Shows:

```bash
Filesystem  Size  Used Avail Use% Mounted on
/dev/sda1   50G   20G   28G  42% /
```

🚨 Warning: Use% > 90%? Time to clean up!

---

3️⃣ free -h

🔹 What it does: Checks RAM + swap usage.
💻 Try it:

```bash
free -h
```

📌 Key metrics:

```bash
              total  used  free
Mem:           7.7G  2.1G  5.6G
Swap:          2.0G  0.1G  1.9G
```

💡 Pro Tip: cat /proc/meminfo for extreme details!

---

4️⃣ top

🔹 What it does: Live dashboard of running processes.
💻 Try it:

```bash
top
```

📌 Press:

· q to quit
· Shift+M to sort by RAM usage

🔎 Better alternative: Install htop for colorful, interactive monitoring!

---

5️⃣ ps aux

🔹 What it does: Snapshots ALL running processes.
💻 Try it:

```bash
ps aux
```

📌 Find specific apps:

```bash
ps aux | grep firefox
```

---

6️⃣ kill -9

🔹 What it does: Force-stops a misbehaving program.
💻 Try it:

1. First find the PID (Process ID):

```bash
ps aux | grep bad_app
```

1. Nuke it:

```bash
kill -9 1234  # Replace 1234 with the actual PID
```

⚠️ Caution: Only use -9 as a last resort!

---

📢 Call-to-Action

✅ Like if you've ever had to kill -9 a frozen app!

🔔 Follow for advanced Linux monitoring tools tomorrow.
