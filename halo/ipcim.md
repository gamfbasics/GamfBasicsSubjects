# IP-cím

- IPv4: 32 bit, 4 oktetben (dotted decimal), pl. `192.168.10.34`
- Alhálózati maszk CIDR-ben: /N ahol N = hálózati bitek száma pl. `/27`
- Hálózati cím = IP AND mask (bitenkénti ÉS)
- Broadcast (IPv4): a hálózat összes bite 1 a host-részen
- Használható hostok száma IPv4-ben: `2^(32 - N) - 2` N = maszk (ha nem /31 vagy /32)
- IPv6: 128 bit, 8 hextet (16 bites darab), pl. `2001:db8::1`

## Gyakori maszkok gyorstáblázat
| Maszk   | Decimális       | kiosztható cím | használható cím |
| ------- | --------------- | :------------: | :-------------: |
| **/24** | 255.255.255.0   | 256            | 254             |
| **/25** | 255.255.255.128 | 128            | 126             |
| **/26** | 255.255.255.192 | 64             | 62              |
| **/27** | 255.255.255.224 | 32             | 30              |
| **/28** | 255.255.255.240 | 16             | 14              |
| **/29** | 255.255.255.248 | 8              | 6               |

## Alhálózat-számítás
| Példa                   | `192.168.10.34/27`                                      |
| ----------------------- | ------------------------------------------------------- |
| IP binárisan            | `11000000.10101000.00001010.00100010`                   |
| Maszk binárisan         | `11111111.11111111.11111111.11100000`                   |
| Hálózati cím            | `11000000.10101000.00001010.00100000` = `192.168.10.32` |
| Broadcast cím           | `11000000.10101000.00001010.00111111` = `192.168.10.63` |
| Első használható host   | `192.168.10.33`                                         |
| Utolsó használható host | `192.168.10.62`                                         |
