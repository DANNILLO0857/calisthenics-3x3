# CALISTHENICS 3×3 — Foundation
## Publicación
1. Crea un repositorio público `calisthenics-3x3` en GitHub.
2. Descomprime el ZIP y sube todos los archivos a la raíz del repositorio.
3. Settings → Pages → Deploy from a branch → main → / (root) → Save.
4. Abre la URL que GitHub Pages muestra. En Safari: Compartir → Añadir a pantalla de inicio.
## Uso
Los datos se guardan en el dispositivo. Exporta copias JSON desde Laboratory. Las semanas se calculan por fecha local; el historial no se borra. Los domingos de descanso no rompen la racha. Los vídeos son enlaces de búsqueda, no vídeos individuales verificados. La movilidad es provisional hasta consultar I Can Run. El modo offline requiere una primera carga online correcta. No incluye notificaciones push; usa recordatorios de iOS. Para actualizar la caché cambia su versión en sw.js.

## V2
Nutrition sustituye Progress en el menú. El historial de fuerza sigue en Laboratory. Los objetivos nutricionales son opcionales y manuales. Para actualizar, exporta una copia y reemplaza los archivos en el mismo repositorio.

## V2.1 Signature Edition
Nuevo icono, firma by Daniel D. y referencia a la fábula. Conserva los datos existentes. Si iOS mantiene el icono anterior, exporta primero una copia de seguridad antes de retirar y volver a añadir la app.

## V3: IA real (configuración necesaria)
1. Exporta tus registros antes de actualizar. Sube los archivos de la app al repositorio habitual; worker.js es para Cloudflare, no necesita subirse a GitHub.
2. En https://aistudio.google.com/apikey crea una clave de un proyecto sin facturación, si la modalidad gratuita está disponible. Elige un modelo Gemini multimodal con cuota gratuita vigente; copia su ID exacto (sin models/).
3. En https://dash.cloudflare.com crea un Worker en el plan gratuito, pega worker.js en su editor y despliega. En Settings > Variables and Secrets configura GEMINI_KEY (secret), ACCESS_CODE (secret, contraseña larga aleatoria), GEMINI_MODEL (texto). Nunca publiques esos secretos en GitHub. No habilites facturación si quieres evitar cargos.
4. En Nutrition > Configurar conexión IA pega la URL HTTPS del Worker y el código. El código se conserva durante la sesión; vuelve a introducirlo si se cierra. Las fotos y preguntas se transmiten a Gemini; revisa sus condiciones de privacidad. Los registros confirmados permanecen locales.
5. Prueba el chat y una foto. Si se agota la cuota, espera o registra manualmente. La IA requiere internet. Las estimaciones son aproximadas y editables. No se ha probado con una clave real.

## V3.1
Firma filosófica: 井底之蛙. Sin cambios en los registros.

## V4.0
Perfil adulto, balance energético, peso y promedio de días registrados. Conserva la clave local de datos. No requiere cambios al Worker. Subir todos los archivos web, incluido balance.js. IA requiere código de acceso y prueba real.

## V4.1
Recordar acceso opcional en el dispositivo y botón Olvidar acceso. El código del Worker se guarda localmente sin cifrar si se activa la opción; no usar en dispositivos compartidos. No se guardan las claves de proveedores en la app. Actualizar ai.js, index.html y sw.js. No requiere cambios en Cloudflare.

V5.0: subir todos los archivos a la raíz del mismo repositorio. Exportar copia JSON antes de actualizar. Running reemplaza Laboratory en navegación; notas y copias siguen accesibles. GPS requiere HTTPS, permisos y pantalla abierta; caminadora usa velocidad manual. Tarjeta PNG con trazado sin mapa base. No hay notificaciones push, frecuencia cardíaca, parciales por km, plan de running ni fotografías nuevas en esta entrega. Kilometraje supone un único par. No se ha probado en iPhone. No cambiar Worker.

## V5.1 Design Edition
Upload all files including the `images/` directory, preserving its structure. Original supplied photos are copied without AI modification. CSS overlays provide the three quotes. To replace a photo, retain its filename or update the CSS and service worker asset list. GitHub Pages is public: only publish photos you have permission to share. Existing localStorage key and AI scripts are unchanged. No new backend or push notifications. GPS background limitations remain. 
