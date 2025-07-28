##  TAREA: Notificación de Fallos de CI en Discord o otra plataforma a tu preferencia con Webhook

###  Enunciado

Crea un pipeline de GitLab CI/CD que simule un fallo en el job de construcción (`build`) y que, en caso de error, envíe automáticamente un mensaje al canal de Discord usando un Webhook.

El mensaje debe incluir:
- Nombre del proyecto.
- Rama donde falló el pipeline.
- Enlace directo al pipeline en GitLab.

El webhook debe estar configurado correctamente como variable de entorno (`DISCORD_WEBHOOK_URL`) en GitLab.

---

### ✅ Requisitos técnicos

- El Webhook de Discord debe estar creado y funcionando.
- La variable `DISCORD_WEBHOOK_URL` debe estar configurada en `Settings > CI/CD > Variables`.
- El mensaje debe enviarse **solo si el pipeline falla**.

---

###  Crear el Webhook
1. Abre Discord y ve al canal donde quieres recibir notificaciones.
2. Haz clic en  **Editar canal** > **Integraciones** > **Webhooks**.
3. Crea un nuevo Webhook.
4. Ponle un nombre (ej. `GitLab Notifier`) y selecciona el canal.
5. Haz clic en **Copiar URL del Webhook**.
