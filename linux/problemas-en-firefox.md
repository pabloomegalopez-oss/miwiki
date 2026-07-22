# Problemas en firefox

> Firefox — problemas de procesos y profile issues

## Descripción

Error: “Firefox se está ejecutando pero no responde”

## Causa
Proceso zombie o instancia previa no cerrada correctamente.

Abrir Monitor del sistema o terminal.

Buscar procesos:

ps aux | grep firefox

## Matar proceso(s):
kill PID
## Si no responde:
kill -9 PID

Reiniciar Firefox.

## Si hay problemas de perfil

Firefox guarda los perfiles en ~/.mozilla/firefox/.

Copiar cert.db, key3.db, secmod.db desde un perfil con firma reconocida al nuevo perfil puede resolver problemas de firma.