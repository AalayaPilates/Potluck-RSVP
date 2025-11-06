
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>End of Year Potluck Celebration</title>
    <link href="https://fonts.googleapis.com/css2?family=Intro:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Intro', 'Arial', sans-serif;
            background: linear-gradient(to bottom, #e8e4dc 0%, #d4cfc4 100%);
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 900px;
            width: 100%;
            margin: 0 auto;
        }
        
        .invitation {
            background: linear-gradient(rgba(232, 228, 220, 0.85), rgba(212, 207, 196, 0.85)),
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 1400"><rect fill="%23e8e4dc" width="800" height="1400"/><circle cx="400" cy="900" r="200" fill="%23f5f0e8" opacity="0.3"/><circle cx="200" cy="400" r="150" fill="%23d4cfc4" opacity="0.2"/><circle cx="600" cy="600" r="180" fill="%23f5f0e8" opacity="0.25"/></svg>');
            background-size: cover;
            background-position: center;
            border-radius: 20px;
            padding: 50px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.15);
            margin-bottom: 30px;
            text-align: center;
            position: relative;
        }
        
        .header-text {
            font-size: 52px;
            font-weight: 400;
            color: #000000;
            margin-bottom: 5px;
            letter-spacing: 2px;
            font-family: 'Intro', sans-serif;
        }
        
        .with-text {
            font-size: 32px;
            color: #000000;
            margin-bottom: 40px;
            font-weight: 300;
            font-family: 'Intro', sans-serif;
        }
        
        .pot-container {
            margin: 0 auto 40px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .pot-svg {
            width: 280px;
            height: 240px;
            filter: drop-shadow(0 8px 20px rgba(139, 46, 46, 0.3));
        }
        
        .event-box {
            background: rgba(255, 255, 255, 0.92);
            padding: 40px 50px;
            border-radius: 25px;
            margin: 35px auto;
            max-width: 580px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.12);
        }
        
        .day-text {
            font-size: 50px;
            font-weight: 700;
            color: #000000;
            margin-bottom: 8px;
            font-family: 'Intro', sans-serif;
        }
        
        .date-text {
            font-size: 58px;
            font-weight: 700;
            color: #000000;
            margin-bottom: 18px;
            font-family: 'Intro', sans-serif;
        }
        
        .date-text sup {
            font-size: 34px;
            vertical-align: super;
        }
        
        .time-text {
            font-size: 44px;
            font-weight: 700;
            color: #000000;
            margin-bottom: 22px;
            font-family: 'Intro', sans-serif;
        }
        
        .location-text {
            font-size: 26px;
            color: #000000;
            font-weight: 400;
            font-family: 'Intro', sans-serif;
        }
        
        .welcome-message {
            background: rgba(240, 235, 225, 0.85);
            padding: 38px;
            border-radius: 18px;
            margin: 32px 0;
            line-height: 1.8;
            text-align: left;
        }
        
        .welcome-message p {
            font-size: 18px;
            color: #4a4a4a;
            margin-bottom: 16px;
            font-family: 'Intro', sans-serif;
        }
        
        .welcome-title {
            color: #8B2E2E;
            font-size: 26px;
            font-weight: 700;
            margin-bottom: 20px;
            text-align: center;
            font-family: 'Intro', sans-serif;
        }
        
        .info-section {
            background: rgba(255, 255, 255, 0.75);
            padding: 28px;
            border-radius: 12px;
            margin: 22px 0;
            text-align: left;
        }
        
        .info-item {
            margin: 14px 0;
            font-size: 18px;
            color: #4a4a4a;
            display: flex;
            align-items: center;
            font-family: 'Intro', sans-serif;
        }
        
        .info-icon {
            margin-right: 12px;
            font-size: 22px;
        }
        
        .door-prize {
            background: #8B2E2E;
            color: white;
            padding: 28px;
            border-radius: 18px;
            margin: 28px 0;
            font-size: 26px;
            font-weight: 700;
            font-family: 'Intro', sans-serif;
        }
        
        .form-section {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 45px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.15);
        }
        
        .form-title {
            font-size: 36px;
            color: #2d2d2d;
            margin-bottom: 35px;
            text-align: center;
            font-weight: 700;
            letter-spacing: 2px;
            font-family: 'Intro', sans-serif;
        }
        
        .form-group {
            margin-bottom: 28px;
        }
        
        label {
            display: block;
            margin-bottom: 10px;
            color: #4a4a4a;
            font-weight: 600;
            font-size: 17px;
            font-family: 'Intro', sans-serif;
        }
        
        input, select {
            width: 100%;
            padding: 14px 18px;
            border: 2px solid #d4cfc4;
            border-radius: 10px;
            font-size: 16px;
            transition: border-color 0.3s;
            background: white;
            font-family: 'Intro', sans-serif;
        }
        
        input:focus, select:focus {
            outline: none;
            border-color: #8B2E2E;
        }
        
        .radio-group {
            display: flex;
            gap: 35px;
            margin-top: 12px;
        }
        
        .radio-option {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .radio-option input[type="radio"] {
            width: auto;
            margin: 0;
            accent-color: #8B2E2E;
        }
        
        .radio-option label {
            margin: 0;
            font-family: 'Intro', sans-serif;
        }
        
        .submit-btn {
            background: #8B2E2E;
            color: white;
            padding: 18px 45px;
            border: none;
            border-radius: 50px;
            font-size: 20px;
            font-weight: 700;
            cursor: pointer;
            width: 100%;
            transition: transform 0.3s, box-shadow 0.3s;
            font-family: 'Intro', sans-serif;
            letter-spacing: 1px;
        }
        
        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 12px 28px rgba(139, 46, 46, 0.4);
            background: #a03838;
        }
        
        .success-message {
            display: none;
            background: #48bb78;
            color: white;
            padding: 22px;
            border-radius: 12px;
            text-align: center;
            margin-top: 22px;
            font-size: 18px;
            font-family: 'Intro', sans-serif;
        }
        
        @media (max-width: 768px) {
            .invitation, .form-section {
                padding: 30px 20px;
            }
            
            .header-text {
                font-size: 38px;
            }
            
            .with-text {
                font-size: 24px;
            }
            
            .pot-svg {
                width: 220px;
                height: 190px;
            }
            
            .day-text {
                font-size: 38px;
            }
            
            .date-text {
                font-size: 44px;
            }
            
            .time-text {
                font-size: 34px;
            }
            
            .location-text {
                font-size: 20px;
            }
            
            .welcome-message p {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Invitation -->
        <div class="invitation">
            <div class="header-text">Lets Celebrate</div>
            <div class="with-text">with</div>
            
            <div class="pot-container">
                <svg class="pot-svg" viewBox="0 0 360 300" xmlns="http://www.w3.org/2000/svg">
                    <defs>
                        <!-- Enhanced gradients for ultra-realistic look -->
                        <radialGradient id="potMainGradient" cx="35%" cy="30%">
                            <stop offset="0%" style="stop-color:#D45D5D;stop-opacity:1" />
                            <stop offset="25%" style="stop-color:#B04545;stop-opacity:1" />
                            <stop offset="60%" style="stop-color:#8B2E2E;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#5B1515;stop-opacity:1" />
                        </radialGradient>
                        <radialGradient id="potDarkGradient" cx="50%" cy="50%">
                            <stop offset="0%" style="stop-color:#8B2E2E;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#4A1010;stop-opacity:1" />
                        </radialGradient>
                        <radialGradient id="lidTopGradient" cx="38%" cy="25%">
                            <stop offset="0%" style="stop-color:#E06B6B;stop-opacity:1" />
                            <stop offset="30%" style="stop-color:#C05050;stop-opacity:1" />
                            <stop offset="70%" style="stop-color:#9B3535;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#7A2525;stop-opacity:1" />
                        </radialGradient>
                        <radialGradient id="handleShine" cx="30%" cy="25%">
                            <stop offset="0%" style="stop-color:#B04545;stop-opacity:1" />
                            <stop offset="50%" style="stop-color:#8B2E2E;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#5B1515;stop-opacity:1" />
                        </radialGradient>
                        <linearGradient id="rimGradient" x1="0%" y1="0%" x2="0%" y2="100%">
                            <stop offset="0%" style="stop-color:#9B3535;stop-opacity:1" />
                            <stop offset="100%" style="stop-color:#6B1E1E;stop-opacity:1" />
                        </linearGradient>
                    </defs>
                    
                    <!-- Soft shadow beneath pot -->
                    <ellipse cx="180" cy="285" rx="130" ry="12" fill="black" opacity="0.25"/>
                    
                    <!-- Left Handle - 3D cylindrical -->
                    <g>
                        <!-- Handle shadow -->
                        <ellipse cx="42" cy="168" rx="22" ry="48" fill="black" opacity="0.15"/>
                        <!-- Handle body -->
                        <ellipse cx="40" cy="165" rx="20" ry="45" fill="url(#handleShine)"/>
                        <!-- Handle connection to pot -->
                        <rect x="58" y="145" width="12" height="40" rx="6" fill="url(#potDarkGradient)"/>
                        <!-- Handle shine -->
                        <ellipse cx="35" cy="158" rx="8" ry="20" fill="white" opacity="0.2"/>
                        <ellipse cx="32" cy="165" rx="5" ry="12" fill="white" opacity="0.15"/>
                    </g>
                    
                    <!-- Right Handle - 3D cylindrical -->
                    <g>
                        <!-- Handle shadow -->
                        <ellipse cx="318" cy="168" rx="22" ry="48" fill="black" opacity="0.15"/>
                        <!-- Handle body -->
                        <ellipse cx="320" cy="165" rx="20" ry="45" fill="url(#handleShine)"/>
                        <!-- Handle connection to pot -->
                        <rect x="290" y="145" width="12" height="40" rx="6" fill="url(#potDarkGradient)"/>
                        <!-- Handle shine -->
                        <ellipse cx="325" cy="158" rx="8" ry="20" fill="white" opacity="0.2"/>
                        <ellipse cx="328" cy="165" rx="5" ry="12" fill="white" opacity="0.15"/>
                    </g>
                    
                    <!-- Pot Body - Bulbous rounded shape -->
                    <!-- Bottom shadow of pot -->
                    <ellipse cx="180" cy="265" rx="95" ry="18" fill="#3A0808" opacity="0.6"/>
                    
                    <!-- Main pot body with curve -->
                    <path d="M 85 135 
                             Q 75 140, 72 160
                             Q 70 200, 75 230
                             Q 80 255, 95 265
                             Q 120 275, 180 278
                             Q 240 275, 265 265
                             Q 280 255, 285 230
                             Q 290 200, 288 160
                             Q 285 140, 275 135 Z" 
                          fill="url(#potMainGradient)"/>
                    
                    <!-- Pot bottom curve -->
                    <ellipse cx="180" cy="270" rx="88" ry="16" fill="#4A1010"/>
                    
                    <!-- Main highlight on pot body -->
                    <ellipse cx="135" cy="180" rx="38" ry="70" fill="white" opacity="0.12"/>
                    <ellipse cx="120" cy="200" rx="25" ry="50" fill="white" opacity="0.08"/>
                    
                    <!-- Secondary highlight -->
                    <ellipse cx="210" cy="210" rx="20" ry="40" fill="white" opacity="0.05"/>
                    
                    <!-- Pot opening/rim -->
                    <ellipse cx="180" cy="135" rx="105" ry="20" fill="#3A0808"/>
                    <ellipse cx="180" cy="133" rx="103" ry="18" fill="#2A0505"/>
                    
                    <!-- Decorative rim band -->
                    <ellipse cx="180" cy="135" rx="108" ry="22" fill="none" stroke="url(#rimGradient)" stroke-width="3" opacity="0.7"/>
                    
                    <!-- Lid - Dome shaped with realistic curve -->
                    <!-- Lid bottom shadow -->
                    <ellipse cx="180" cy="125" rx="115" ry="18" fill="black" opacity="0.2"/>
                    
                    <!-- Lid dome structure -->
                    <ellipse cx="180" cy="100" rx="112" ry="35" fill="url(#lidTopGradient)"/>
                    <path d="M 68 100 Q 68 70, 180 60 Q 292 70, 292 100 Z" fill="url(#lidTopGradient)"/>
                    
                    <!-- Lid base rim -->
                    <ellipse cx="180" cy="120" rx="115" ry="18" fill="url(#lidTopGradient)"/>
                    
                    <!-- Lid highlights for shine -->
                    <ellipse cx="145" cy="82" rx="50" ry="20" fill="white" opacity="0.15"/>
                    <ellipse cx="135" cy="95" rx="35" ry="15" fill="white" opacity="0.1"/>
                    <ellipse cx="200" cy="105" rx="25" ry="10" fill="white" opacity="0.06"/>
                    
                    <!-- Lid edge highlight -->
                    <ellipse cx="180" cy="120" rx="110" ry="16" fill="none" stroke="#E06B6B" stroke-width="2" opacity="0.3"/>
                    
                    <!-- Knob - Rounded mushroom shape -->
                    <!-- Knob base shadow -->
                    <ellipse cx="180" cy="75" rx="24" ry="9" fill="black" opacity="0.3"/>
                    
                    <!-- Knob stem -->
                    <ellipse cx="180" cy="65" rx="16" ry="12" fill="url(#potDarkGradient)"/>
                    <rect x="164" y="58" width="32" height="14" fill="url(#potDarkGradient)"/>
                    
                    <!-- Knob top (mushroom cap) -->
                    <ellipse cx="180" cy="50" rx="22" ry="12" fill="url(#lidTopGradient)"/>
                    <ellipse cx="180" cy="48" rx="20" ry="10" fill="url(#handleShine)"/>
                    
                    <!-- Knob highlight -->
                    <ellipse cx="172" cy="47" rx="10" ry="6" fill="white" opacity="0.3"/>
                    <ellipse cx="175" cy="50" rx="6" ry="4" fill="white" opacity="0.2"/>
                    
                    <!-- Text background for better contrast -->
                    <ellipse cx="180" cy="195" rx="95" ry="32" fill="black" opacity="0.18"/>
                    
                    <!-- Text: Potluck with enhanced styling -->
                    <text x="180" y="210" 
                          font-family="'Brush Script MT', 'Segoe Script', 'Lucida Handwriting', cursive" 
                          font-size="62" 
                          fill="white" 
                          text-anchor="middle" 
                          font-style="italic" 
                          font-weight="normal"
                          style="text-shadow: 3px 3px 6px rgba(0,0,0,0.4), -1px -1px 2px rgba(255,255,255,0.1);">
                        Potluck
                    </text>
                </svg>
            </div>
            
            <div class="event-box">
                <div class="day-text">Sunday</div>
                <div class="date-text">7<sup>th</sup> Dec 2025</div>
                <div class="time-text">Start 13:00</div>
                <div class="location-text">at BASI Pilates Indonesia HQ</div>
            </div>
            
            <div class="welcome-message">
                <div class="welcome-title">Let's Celebrate With Us!</div>
                <p>
                    As we close this wonderful year together, we warmly invite you to join our Aalaya Pilates and BASI Pilates Indonesia family for an afternoon of joy, connection, and gratitude.
                </p>
                <p>
                    This is more than just a gathering—it's a celebration of <strong>community and togetherness</strong>. We've grown stronger through shared moments, laughter, and support. Let's come together once more to honor the bonds we've built and create new memories.
                </p>
                <p>
                    Bring your favorite dish, bring your warmth, and most importantly, bring yourself! Whether you're sharing a home-cooked specialty or simply your presence and smile, you are the heart of this celebration.
                </p>
                <p style="font-style: italic; margin-bottom: 0;">
                    We can't wait to see you, share stories, dance together, and celebrate the beautiful community we've built. Your presence will make this day truly special! ✨
                </p>
            </div>
            
            <div class="info-section">
                <div class="info-item">
                    <span class="info-icon">🎉</span>
                    <span>Meet & Greet with friends and colleagues</span>
                </div>
                <div class="info-item">
                    <span class="info-icon">💃</span>
                    <span>Dance and celebrate together</span>
                </div>
                <div class="info-item">
                    <span class="info-icon">🍽️</span>
                    <span>Share your favorite dishes</span>
                </div>
            </div>
            
            <div class="door-prize">
                🎁 Exciting Door Prizes Await! 🎁
            </div>
        </div>
        
        <!-- RSVP Form -->
        <div class="form-section">
            <h2 class="form-title">RSVP FORM</h2>
            
            <form id="rsvpForm">
                <div class="form-group">
                    <label for="name">Full Name *</label>
                    <input type="text" id="name" name="name" required>
                </div>
                
                <div class="form-group">
                    <label for="email">Email Address *</label>
                    <input type="email" id="email" name="email" required>
                </div>
                
                <div class="form-group">
                    <label for="guests">Number of People Attending *</label>
                    <input type="number" id="guests" name="guests" min="1" max="10" required>
                </div>
                
                <div class="form-group">
                    <label>Will you bring food? *</label>
                    <div class="radio-group">
                        <div class="radio-option">
                            <input type="radio" id="foodYes" name="bringFood" value="yes" required>
                            <label for="foodYes">Yes, I'll bring food</label>
                        </div>
                        <div class="radio-option">
                            <input type="radio" id="foodNo" name="bringFood" value="no" required>
                            <label for="foodNo">No</label>
                        </div>
                    </div>
                </div>
                
                <div class="form-group" id="portionGroup" style="display: none;">
                    <label for="portions">How many portions? *</label>
                    <input type="number" id="portions" name="portions" min="1" max="50">
                </div>
                
                <button type="submit" class="submit-btn">Submit RSVP</button>
                
                <div class="success-message" id="successMessage">
                    ✓ Thank you! Your RSVP has been submitted successfully. We look forward to seeing you!
                </div>
            </form>
        </div>
    </div>
    
    <script>
        const form = document.getElementById('rsvpForm');
        const foodYes = document.getElementById('foodYes');
        const foodNo = document.getElementById('foodNo');
        const portionGroup = document.getElementById('portionGroup');
        const portionsInput = document.getElementById('portions');
        const successMessage = document.getElementById('successMessage');
        
        // IMPORTANT: Replace this URL with your Google Apps Script deployment URL
        const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/AKfycbwAcx3HfW8hDS4cGtIAFnF-oMX2q0jI_g5xAAwpOWgFDwGLo7p53_s_FJtXw4IiNp9G/exec";
        
        foodYes.addEventListener('change', function() {
            if (this.checked) {
                portionGroup.style.display = 'block';
                portionsInput.required = true;
            }
        });
        
        foodNo.addEventListener('change', function() {
            if (this.checked) {
                portionGroup.style.display = 'none';
                portionsInput.required = false;
                portionsInput.value = '';
            }
        });
        
        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const submitBtn = form.querySelector('.submit-btn');
            const originalText = submitBtn.textContent;
            submitBtn.textContent = 'Submitting...';
            submitBtn.disabled = true;
            
            const formData = {
                name: document.getElementById('name').value,
                email: document.getElementById('email').value,
                guests: document.getElementById('guests').value,
                bringFood: document.querySelector('input[name="bringFood"]:checked').value,
                portions: portionsInput.value || 'N/A',
                timestamp: new Date().toLocaleString()
            };
            
            // Send to Google Sheets
            fetch(GOOGLE_SCRIPT_URL, {
                method: 'POST',
                mode: 'no-cors',
                headers: {
                    'Content-Type': 'application/json',
                },
                body: JSON.stringify(formData)
            })
            .then(() => {
                console.log('RSVP Submitted:', formData);
                successMessage.style.display = 'block';
                form.reset();
                portionGroup.style.display = 'none';
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
                
                successMessage.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
                
                setTimeout(function() {
                    successMessage.style.display = 'none';
                }, 5000);
            })
            .catch((error) => {
                console.error('Error:', error);
                alert('There was an error submitting your RSVP. Please try again or contact us directly.');
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            });
        });
    </script>
</body>
</html>
