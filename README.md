# Avinya-ayurvedaa<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avinya Ayurveda - Prakriti Analyzer</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="background-leaf">☘️</div>
    <div class="app-container">
        <header>
            <h1>🌿 Avinya Ayurveda</h1>
            <p class="subtitle">Discover Your Ayurvedic Prakriti</p>
        </header>

        <div class="progress-wrapper">
            <div class="progress-container">
                <div id="progress-bar"></div>
            </div>
            <div id="progress-text">0%</div>
        </div>

        <div id="step-1" class="step active">
            <h2>Physical Constitution 👤</h2>
            <span class="category-title">1. Body Frame</span>
            <label class="option"><input type="radio" name="frame" data-dosha="vata"> Lean, lanky, or very tall/short</label>
            <label class="option"><input type="radio" name="frame" data-dosha="pitta"> Medium build; symmetrical and muscular</label>
            <label class="option"><input type="radio" name="frame" data-dosha="kapha"> Large, broad, or stocky build</label>

            <span class="category-title">2. Skin Texture</span>
            <label class="option"><input type="radio" name="skin" data-dosha="vata"> Dry, rough, or cool to the touch</label>
            <label class="option"><input type="radio" name="skin" data-dosha="pitta"> Warm, sensitive, reddish or freckled</label>
            <label class="option"><input type="radio" name="skin" data-dosha="kapha"> Smooth, oily, thick, and cool</label>

            <span class="category-title">3. Hair Quality</span>
            <label class="option"><input type="radio" name="hair" data-dosha="vata"> Dry, brittle, curly, or frizzy</label>
            <label class="option"><input type="radio" name="hair" data-dosha="pitta"> Fine, soft; early thinning or graying</label>
            <label class="option"><input type="radio" name="hair" data-dosha="kapha"> Thick, oily, wavy, and strong</label>

            <span class="category-title">4. Joints & Bones</span>
            <label class="option"><input type="radio" name="joints" data-dosha="vata"> Prominent joints; cracking sounds</label>
            <label class="option"><input type="radio" name="joints" data-dosha="pitta"> Moderate joints; flexible and loose</label>
            <label class="option"><input type="radio" name="joints" data-dosha="kapha"> Hidden joints; sturdy and well-knit</label>

            <span class="category-title">5. Eye Appearance</span>
            <label class="option"><input type="radio" name="eyes" data-dosha="vata"> Small, dry, or sunken; frequent blinking</label>
            <label class="option"><input type="radio" name="eyes" data-dosha="pitta"> Sharp, penetrating; sensitive to light</label>
            <label class="option"><input type="radio" name="eyes" data-dosha="kapha"> Large, attractive, with thick lashes</label>
            <button onclick="nextStep(2)">Next: Physiological Rhythms</button>
        </div>

        <div id="step-2" class="step">
            <h2>Biological Functions ⚡</h2>
            <span class="category-title">6. Appetite & Digestion</span>
            <label class="option"><input type="radio" name="appetite" data-dosha="vata"> Irregular; sometimes hungry/not</label>
            <label class="option"><input type="radio" name="appetite" data-dosha="pitta"> Intense; irritable if meal is delayed</label>
            <label class="option"><input type="radio" name="appetite" data-dosha="kapha"> Steady but low; can skip meals</label>

            <span class="category-title">7. Bowel Habits</span>
            <label class="option"><input type="radio" name="bowels" data-dosha="vata"> Hard/dry stools; prone to constipation</label>
            <label class="option"><input type="radio" name="bowels" data-dosha="pitta"> Regular; prone to loose motions</label>
            <label class="option"><input type="radio" name="bowels" data-dosha="kapha"> Regular; heavy, slow, or oily stools</label>

            <span class="category-title">8. Sleep Quality</span>
            <label class="option"><input type="radio" name="sleep" data-dosha="vata"> Light sleeper; easily disturbed</label>
            <label class="option"><input type="radio" name="sleep" data-dosha="pitta"> Sound sleeper for moderate durations</label>
            <label class="option"><input type="radio" name="sleep" data-dosha="kapha"> Deep, heavy sleep; hard to wake</label>

            <span class="category-title">9. Weather Preference</span>
            <label class="option"><input type="radio" name="weather" data-dosha="vata"> Dislikes cold; loves the sun</label>
            <label class="option"><input type="radio" name="weather" data-dosha="pitta"> Dislikes heat; loves cool spaces</label>
            <label class="option"><input type="radio" name="weather" data-dosha="kapha"> Dislikes damp; prefers dry warmth</label>

            <span class="category-title">10. Stamina & Energy</span>
            <label class="option"><input type="radio" name="stamina" data-dosha="vata"> High energy bursts; tires quickly</label>
            <label class="option"><input type="radio" name="stamina" data-dosha="pitta"> Moderate, focused; competitive</label>
            <label class="option"><input type="radio" name="stamina" data-dosha="kapha"> High steady stamina; slow to start</label>
            <button onclick="nextStep(3)">Next: Mind & Personality</button>
        </div>

        <div id="step-3" class="step">
            <h2>Mind & Behavior 🧠</h2>
            <span class="category-title">11. Speech Style</span>
            <label class="option"><input type="radio" name="speech" data-dosha="vata"> Fast, talkative, wanders off-topic</label>
            <label class="option"><input type="radio" name="speech" data-dosha="pitta"> Sharp, logical, convincing</label>
            <label class="option"><input type="radio" name="speech" data-dosha="kapha"> Slow, steady, pleasant</label>

            <span class="category-title">12. Memory</span>
            <label class="option"><input type="radio" name="memory" data-dosha="vata"> Learns quickly, forgets quickly</label>
            <label class="option"><input type="radio" name="memory" data-dosha="pitta"> Moderate; long retention of logic</label>
            <label class="option"><input type="radio" name="memory" data-dosha="kapha"> Slow to learn, but never forgets</label>

            <span class="category-title">13. Stress Response</span>
            <label class="option"><input type="radio" name="stress" data-dosha="vata"> Becomes anxious or fearful</label>
            <label class="option"><input type="radio" name="stress" data-dosha="pitta"> Becomes angry or impatient</label>
            <label class="option"><input type="radio" name="stress" data-dosha="kapha"> Remains calm or withdrawn</label>

            <span class="category-title">14. Decisions</span>
            <label class="option"><input type="radio" name="decisions" data-dosha="vata"> Indecisive; changes mind often</label>
            <label class="option"><input type="radio" name="decisions" data-dosha="pitta"> Fast, decisive, authoritative</label>
            <label class="option"><input type="radio" name="decisions" data-dosha="kapha"> Slow and cautious; deliberate</label>

            <span class="category-title">15. Spending</span>
            <label class="option"><input type="radio" name="money" data-dosha="vata"> Spends impulsively</label>
            <label class="option"><input type="radio" name="money" data-dosha="pitta"> Spends on luxury/quality</label>
            <label class="option"><input type="radio" name="money" data-dosha="kapha"> Saves; spends only on needs</label>
            <button onclick="calculateResults()">Generate My Roadmap</button>
        </div>

        <div id="step-4" class="step">
            <div id="result-summary"></div>
            <div id="roadmap-content"></div>
            <button onclick="window.print()" style="background:#444;">Download PDF Roadmap 📄</button>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
:root { --primary: #6b8e23; --bg: #fdfaf5; --text: #333; }
body { font-family: 'Poppins', sans-serif; background: #fdfaf5; color: var(--text); padding: 20px; display: flex; justify-content: center; }
.app-container { max-width: 600px; width: 100%; }
header { text-align: center; }
h1 { color: var(--primary); }
.progress-container { background: #e0e0e0; border-radius: 10px; height: 10px; overflow: hidden; }
#progress-bar { width: 0%; height: 100%; background: var(--primary); transition: 0.3s; }
.step { display: none; background: white; padding: 25px; border-radius: 20px; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
.active { display: block; }
.category-title { display: block; font-weight: 700; margin-top: 15px; font-size: 0.8rem; color: #777; text-transform: uppercase; }
.option { display: block; padding: 10px; border: 1px solid #eee; border-radius: 8px; margin-top: 5px; cursor: pointer; }
button { width: 100%; padding: 15px; background: var(--primary); color: white; border: none; border-radius: 10px; font-weight: 600; cursor: pointer; margin-top: 20px; }
.consult-btn { display: inline-block; background: var(--primary); color: white; padding: 10px 20px; border-radius: 25px; text-decoration: none; font-weight: 600; margin-top: 15px; }
