# TriviLol

**Trivia de historia y campeones inspirada en League of Legends**, donde cada respuesta correcta te acerca a desbloquear ilustraciones únicas de campeones.  
Aprende, demuestra tus conocimientos y gana campeones al estilo de un juego de fantasía interactivo.

---

## 🎯 Descripción general

**Historia & Campeones** es una aplicación de trivia creada con **Flutter + Dart**, diseñada para poner a prueba tus conocimientos de **lore** y **gameplay competitivo** del universo de *League of Legends*.

Cada respuesta correcta suma puntos, y cada 3 puntos desbloqueas un nuevo **campeón ilustrado**, con animaciones y sonidos temáticos.

---

## 🕹️ Características principales

- **Preguntas de lore y gameplay:** Basadas en la historia y mecánicas del LoL.
- **Sistema de puntos:** +1 por acierto, 0 por fallo.
- **Desbloqueo de campeones:** Cada 3 aciertos desbloquea uno nuevo.
- **Animaciones:** Efectos visuales al acertar o fallar.
- **Sonido temático:**
    - Sonido de torre al fallar.
    - "Derrota" si pierdes todas las vidas.
    - "Victoria" al completar la trivia.
- **Guía interactiva con Yuumi 🐱✨**, que enseña cómo jugar.

---

## 🎨 Campeones

### Campeones iniciales:
- Miss Fortune
- Maestro Yi
- Darius
- Ahri
- Morgana

### Campeones desbloqueables (gachapon):
- Syndra
- Veigar
- Evelynn
- Viego
- Sett
- Margarita
- Teemo
- Yasuo
- Yone
- Se irán añadiendo más en cada versión

---

## 📱 Pantallas principales

### 🏠 **Pantalla de inicio**
- Logo de la app
- Botón **“Jugar”**
- Puntaje total visible

### ❓ **Pantalla de trivia**
- Muestra la pregunta actual
- 4 opciones interactivas
- Animación al acertar o fallar
- Sonidos temáticos

### 🏆 **Pantalla de resultados**
- Muestra el puntaje obtenido
- Campeones desbloqueados con mini animaciones
- Botón para reiniciar o volver al inicio

---

## ⚙️ Stack tecnológico

- **Flutter** — Framework principal
- **Dart** — Lenguaje base
- **Provider** — Manejo de estado
- **Lottie / AnimatedContainer** — Animaciones
- **Assets locales (PNG / SVG / WEBP)** — Campeones e íconos

---

lib/
│
├── main.dart                # Punto de entrada de la app, define la navegación/tab bar
│
├── screens/
│   ├── home_screen.dart     # Pantalla de inicio
│   ├── trivia_screen.dart   # Pantalla de preguntas
│   ├── results_screen.dart  # Pantalla de resultados
│   ├── profile_screen.dart  # Pantalla de perfil editable
│   └── gachapon_screen.dart # Pantalla del gachapon (tiradas y recompensas)
│
├── data/
│   └── questions.dart       # Lista de preguntas y respuestas
│
├── models/
│   ├── champion_model.dart  # Modelo de campeón (nombre, imagen, desbloqueado)
│   └── user_model.dart      # Modelo de usuario (nombre, avatar, puntaje)
│
├── providers/
│   └── game_state.dart      # Provider centralizado para puntaje, campeones, usuario
│
├── widgets/
│   ├── question_card.dart   # Widget para mostrar pregunta + opciones
│   ├── champion_card.dart   # Widget visual para campeones desbloqueados
│   └── gachapon_card.dart   # Widget para mostrar resultados del gachapon
│
└── assets/
├── images/              # Campeones, iconos de usuario, fondos
├── sounds/              # Efectos de sonido
└── animations/          # Archivos Lottie
