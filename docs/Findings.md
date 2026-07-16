# Findings

## Summary

The investigation confirmed unauthorized administrative activity.

---

## Findings

### Finding 1

The account **Omar** was granted sudo privileges.

---

### Finding 2

A successful SSH login originated from the attacker machine.

---

### Finding 3

The account **door** was created remotely.

---

### Finding 4

The **door** account was added to the sudo group.

---

### Finding 5

A password was configured for the new account.

---

### Finding 6

The attacker switched from Omar to the door account.

---

### Finding 7

Authentication logs had been cleared.

---

### Finding 8

Journal logs successfully reconstructed the attack timeline.

---

## Conclusion

The attacker established a persistent administrative backdoor through the creation of the **door** account.
