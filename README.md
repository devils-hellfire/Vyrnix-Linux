# Vyrnix Linux

**Vyrnix Linux** is a minimal, modular Linux distribution inspired by the clarity of FreeBSD and the flexibility of Arch Linux.

The goal:  
👉 A lean system that **adapts automatically to your hardware**  
👉 Maximum control without unnecessary complexity  
👉 Clean structure instead of hidden behavior  

---

## 🧭 Philosophy

Vyrnix combines two proven approaches:

### 🧱 BSD Philosophy
- Clear separation of components
- Strong modular design
- Predictable system behavior
- Focus on simplicity and control

### ⚙️ Arch Linux Principles
- KISS (Keep It Simple, Stupid)
- Rolling release model
- User-centric control
- Minimal defaults, maximum flexibility

---

## 🧩 Architecture

Vyrnix is not a traditional monolithic distribution:

- 🔹 **Modular system design** (inspired by FreeBSD) :contentReference[oaicite:0]{index=0}  
- 🔹 Based on Arch Linux as a foundation :contentReference[oaicite:1]{index=1}  
- 🔹 Custom package structure (`vyrnix-*`)  
- 🔹 Dedicated repository for kernel and modules  

---

## 🚀 Core Concept

### 1. Minimal Base Kernel

A deliberately reduced kernel:

- ❌ No debugging features  
- ❌ No audit system  
- ❌ No unnecessary power-saving features  
- ❌ No generic unused drivers  
- ✅ Only essentials: boot, networking, core functionality  

➡️ Goal: **Maximum performance with minimal complexity**

Included optimizations:

- Kyber / BFQ I/O scheduler  
- PDS process scheduler  
- 1000Hz high-resolution scheduling  
- Hard kernel preemption  
- TCP BBR2 congestion control  

:contentReference[oaicite:2]{index=2}

---

### 2. Post-Install Hardware Detection

After first boot:

1. Hardware scan is executed  
2. Only required modules are installed  
3. System remains minimal and efficient  

Example:
