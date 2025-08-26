# greece-honeymoon
<!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Justin & Shay's Greece Honeymoon</title> <style> * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        line-height: 1.6;
        color: #2c3e50;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        min-height: 100vh;
    }
    
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px;
    }
    
    .header {
        text-align: center;
        color: white;
        margin-bottom: 30px;
        padding: 30px 0;
    }
    
    .header h1 {
        font-size: 3rem;
        margin-bottom: 10px;
        text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    }
    
    .header .subtitle {
        font-size: 1.3rem;
        opacity: 0.9;
    }
    
    .trip-overview {
        background: white;
        border-radius: 15px;
        padding: 25px;
        margin-bottom: 25px;
        box-shadow: 0 8px 25px rgba(0,0,0,0.15);
    }
    
    .overview-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 20px;
        margin-top: 20px;
    }
    
    .overview-card {
        background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
        color: white;
        padding: 20px;
        border-radius: 12px;
        text-align: center;
    }
    
    .overview-card h3 {
        margin-bottom: 10px;
        font-size: 1.1rem;
    }
    
    .day-section {
        background: white;
        border-radius: 15px;
        margin-bottom: 25px;
        overflow: hidden;
        box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        transition: transform 0.3s ease;
    }
    
    .day-section:hover {
        transform: translateY(-5px);
    }
    
    .day-header {
        background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
        color: white;
        padding: 20px;
        cursor: pointer;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    
    .day-header h2 {
        font-size: 1.4rem;
    }
    
    .toggle-arrow {
        font-size: 1.5rem;
        transition: transform 0.3s ease;
    }
    
    .day-content {
        padding: 25px;
        display: none;
    }
    
    .day-content.active {
        display: block;
    }
    
    .location-badge {
        display: inline-block;
        background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
        color: #2c3e50;
        padding: 8px 16px;
        border-radius: 20px;
        font-size: 0.9rem;
        font-weight: bold;
        margin-bottom: 15px;
    }
    
    .activity-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
        margin-top: 20px;
    }
    
    .activity-card {
        background: #f8f9fa;
        border-left: 5px solid #4facfe;
        padding: 20px;
        border-radius: 8px;
    }
    
    .activity-time {
        background: #4facfe;
        color: white;
        padding: 5px 12px;
        border-radius: 15px;
        font-size: 0.9rem;
        font-weight: bold;
        display: inline-block;
        margin-bottom: 10px;
    }
    
    .activity-title {
        font-weight: bold;
        color: #2c3e50;
        margin-bottom: 8px;
    }
    
    .activity-details {
        color: #666;
        font-size: 0.95rem;
    }
    
    .reservation-highlight {
        background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
        border-left: 5px solid #f39c12;
        padding: 15px;
        border-radius: 8px;
        margin: 15px 0;
    }
    
    .confirmation-code {
        font-family: 'Courier New', monospace;
        background: #2c3e50;
        color: #ecf0f1;
        padding: 5px 10px;
        border-radius: 5px;
        font-weight: bold;
    }
    
    .hotel-info {
        background: linear-gradient(135deg, #d299c2 0%, #fef9d7 100%);
        padding: 20px;
        border-radius: 12px;
        margin: 15px 0;
    }
    
    .hotel-name {
        font-size: 1.2rem;
        font-weight: bold;
        color: #2c3e50;
        margin-bottom: 8px;
    }
    
    .contact-info {
        background: #e8f5e8;
        border-left: 5px solid #27ae60;
        padding: 15px;
        border-radius: 8px;
        margin: 15px 0;
    }
    
    .flight-info {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        padding: 20px;
        border-radius: 12px;
        margin: 15px 0;
    }
    
    .footer {
        background: white;
        border-radius: 15px;
        padding: 25px;
        margin-top: 30px;
        text-align: center;
        box-shadow: 0 8px 25px rgba(0,0,0,0.1);
    }
    
    .emergency-contacts {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 15px;
        margin-top: 20px;
    }
    
    @media (max-width: 768px) {
        .header h1 {
            font-size: 2rem;
        }
        
        .header .subtitle {
            font-size: 1.1rem;
        }
        
        .day-header {
            padding: 15px;
        }
        
        .day-content {
            padding: 20px;
        }
        
        .activity-grid {
            grid-template-columns: 1fr;
        }
    }
</style>
</head> <body> <div class="container"> <div class="header"> <h1>Greece Honeymoon</h1> <div class="subtitle">Justin & Shay • September 26 - October 10, 2025</div> </div>
    <div class="trip-overview">
        <h2>Trip Overview</h2>
        <div class="overview-grid">
            <div class="overview-card">
                <h3>Duration</h3>
                <div>15 Days, 14 Nights</div>
            </div>
            <div class="overview-card">
                <h3>Islands</h3>
                <div>Santorini • Naxos • Crete</div>
            </div>
            <div class="overview-card">
                <h3>Activities</h3>
                <div>Sunsets • Sailing • Beaches • Culture</div>
            </div>
            <div class="overview-card">
                <h3>Travel Agent</h3>
                <div>Lori Oliveira - FORA</div>
            </div>
        </div>
    </div>
    <!-- OUTBOUND FLIGHT -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>September 26 - Departure Boston</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <div class="flight-info">
                <div class="activity-title">Flight BOS → JTR</div>
                <div><strong>Departure:</strong> 5:15 PM from Boston Logan</div>
                <div><strong>Arrival:</strong> 12:40 PM+1 in Santorini</div>
                <div><strong>Airlines:</strong> Delta/Air France</div>
                <div><strong>Flights:</strong> DL 8399 → DL 8295 (Paris layover)</div>
                <div><strong>Confirmation:</strong> <span class="confirmation-code">GUUKWU</span></div>
            </div>
            <div class="contact-info">
                <strong>Pre-Travel Checklist:</strong><br>
                • Passports ready<br>
                • International phone plan activated<br>
                • Credit card companies notified<br>
                • Travel adapters packed
            </div>
        </div>
    </div>
    <!-- SANTORINI DAYS -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>September 27 - Arrival & Oia Sunset</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">SANTORINI - Day 1</span>
            <div class="hotel-info">
                <div class="hotel-name">WeSense Santorini</div>
                <div>Imerovigli, Santorini • 2 nights</div>
                <div>Confirmation: <span class="confirmation-code">72954207120081</span></div>
            </div>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">12:40 PM</div>
                    <div class="activity-title">Arrival at JTR Airport</div>
                    <div class="activity-details">Land in Santorini</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">1:00 PM</div>
                    <div class="activity-title">First Meal</div>
                    <div class="activity-details">Lunch at Avocado, The Athenian House, or caldera view drinks at Le Moustache/Vezené</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">3:00 PM</div>
                    <div class="activity-title">Hotel Check-in</div>
                    <div class="activity-details">WeSense & freshen up</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">5:00 PM</div>
                    <div class="activity-title">Oia Adventure</div>
                    <div class="activity-details">Pre-booked taxi to Oia, explore blue domes & Byzantine Castle for sunset</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>6:30 PM - Dinner Reservation</strong><br>
                <strong>Oia Gefsis</strong> - Rooftop dining with sunset views
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>September 28 - Catamaran Sailing</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">SANTORINI - Day 2</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Slow Start</div>
                    <div class="activity-details">Breakfast at WeSense with caldera views</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">2:05 PM</div>
                    <div class="activity-title">Catamaran Pickup</div>
                    <div class="activity-details">Bus pickup at Imerovigli Pharmacy/Sunbird Car Rental</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>3:00 PM - 8:00 PM - Santorini Sailing Sunset Cruise</strong><br>
                • Ammoudi Bay embarkation<br>
                • Swimming & snorkeling at Saint Nicholas<br>
                • Swimming at Thirassia<br>
                • Hot Springs & BBQ onboard<br>
                • Sunset by Venetian Lighthouse<br>
                • Includes dinner & drinks onboard
            </div>
            
            <div class="contact-info">
                <strong>Evening Options:</strong> Relax at hotel or explore Fira (PK Cocktail Bar, Tango, or visit Skaros Rock)
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>September 29 - Travel to Naxos</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">SANTORINI → NAXOS</span>
            
            <div class="flight-info">
                <div class="activity-title">Champion Jet Ferry</div>
                <div><strong>Departure:</strong> 8:20 AM from Santorini</div>
                <div><strong>Arrival:</strong> 9:55 AM in Naxos</div>
                <div><strong>Booking Reference:</strong> <span class="confirmation-code">1112EKUZN</span></div>
            </div>
            
            <div class="hotel-info">
                <div class="hotel-name">Liana Beach Hotel & Spa</div>
                <div>Agios Prokopios Beach, Naxos • 4 nights</div>
                <div>Confirmation: <span class="confirmation-code">72954212916608</span></div>
            </div>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Beach & Old Town</div>
                    <div class="activity-details">Relax at Agios Prokopios Beach, walk through Chora (Old Town & Kastro), visit Portara for sunset</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>7:00 PM - Dinner Reservation</strong><br>
                <strong>Doukato</strong> (Chora) - Outdoor courtyard seating
            </div>
        </div>
    </div>
    <!-- NAXOS DAYS -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>September 30 - Naxos Beach Day</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">NAXOS - Day 2</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Agios Prokopios Beach</div>
                    <div class="activity-details">Beach relaxation, optional paddleboarding</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Lunch</div>
                    <div class="activity-title">Plaka Beach</div>
                    <div class="activity-details">Seaside taverna: Yazoo Beach, Nikos Taverna, or Kahlua Beach Bar</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Optional: Mikri Viglia Beach</div>
                    <div class="activity-details">Beautiful beach alternative or continue at current location</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>8:30 PM - Dinner Reservation</strong><br>
                <strong>Taverna Naxos</strong> (close to hotel)
            </div>
            
            <div class="contact-info">
                <strong>Evening:</strong> Stroll through Chora or drinks at The Soul Kitchen
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 1 - Beach & Mountain Villages</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">NAXOS - Day 3</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Agia Anna or Hawaii Beach</div>
                    <div class="activity-details">Beach time with optional paddleboarding</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Lunch</div>
                    <div class="activity-title">Beachside Dining</div>
                    <div class="activity-details">Taverna Faros, Ostria Cafe, Banana Beach Bar, or Akti Seaside Cafe</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Mountain Villages</div>
                    <div class="activity-details">Visit traditional villages Filoti & Apeiranthos</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>6:00 PM - Dinner Reservation</strong><br>
                <strong>Rotunda</strong> - Sunset view dining
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 2 - Adventure & Culture</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">NAXOS - Day 4</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Rhina Cave Kayaking</div>
                    <div class="activity-details">Explore sea caves & hidden beaches (book on-site)</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Funky Hops Brewery</div>
                    <div class="activity-details">Local craft beer tasting</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Evening</div>
                    <div class="activity-title">Shopping in Chora</div>
                    <div class="activity-details">Browse local shops and souvenirs</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>8:30 PM - Dinner Reservation</strong><br>
                <strong>To Elliniko</strong>
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 3 - Travel to Crete</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">NAXOS → CRETE</span>
            
            <div class="flight-info">
                <div class="activity-title">Flight to Crete</div>
                <div><strong>Departure:</strong> 12:45 PM from Naxos</div>
                <div><strong>Route:</strong> Naxos → Athens layover → Crete</div>
                <div><strong>Arrival:</strong> 3:30 PM in Crete</div>
            </div>
            
            <div class="hotel-info">
                <div class="hotel-name">Elia Zampeliou Hotel (Adults Only)</div>
                <div>32 Zampeliou, Chania • 3 nights</div>
                <div>Confirmation: <span class="confirmation-code">72954214795619</span></div>
            </div>
            
            <div class="contact-info">
                <strong>Car Rental Pickup:</strong> Europcar - Confirmation <span class="confirmation-code">73062353442813</span>
            </div>
            
            <div class="reservation-highlight">
                <strong>9:30 PM - Dinner Reservation</strong><br>
                <strong>Pallas Thealassa Rooftop</strong> Chania (5-minute walk from hotel)
            </div>
        </div>
    </div>
    <!-- CHANIA DAYS -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 4 - Beach & Cooking Class</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">CHANIA - Day 2</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Beach Day</div>
                    <div class="activity-details">Visit Marathi Beach or Seitan Limania Beach</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Lunch</div>
                    <div class="activity-title">Seaside Taverna</div>
                    <div class="activity-details">Lunch at Marathi Beach</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>3:00 PM - Cretan Cooking Class</strong><br>
                <strong>Vamos Traditional Village</strong><br>
                4-hour experience with wine and dinner included
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 5 - Chania Exploration</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">CHANIA - Day 3</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Old Town & Harbor</div>
                    <div class="activity-details">Explore Chania Old Town, Venetian Harbor, local shops, coffee at Koukouvaya</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Optional Midday</div>
                    <div class="activity-title">Theriso Gorge Drive</div>
                    <div class="activity-details">25-min scenic drive, lunch at Ntounias Tavern in Theriso village</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Waterfront Drinks</div>
                    <div class="activity-details">Tabakaria area, Boheme, or Pallas Café-Bar with sea views</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>Dinner: Raki Ba Raki</strong><br>
                Casual, meze-style plates
            </div>
            
            <div class="contact-info">
                <strong>Chania Nightlife (Walking Distance):</strong><br>
                • Fagotto Jazz Bar (live music)<br>
                • Monastiri Cocktail Bar (trendy with views)<br>
                • KLIK Bar (bright, loud music)<br>
                • Sinagogi Bar (chill courtyard)<br>
                • Boheme (sophisticated lounge)
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 6 - Spa & Travel to Heraklion</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">CHANIA → HERAKLION</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Luxury Spa</div>
                    <div class="activity-details">Consider Kensho, Casa Delfino, or Euphoria in Heraklion<br>Jacuzzi/sauna for Justin, massage for Shay</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-time">Afternoon</div>
                    <div class="activity-title">Drive to Heraklion</div>
                    <div class="activity-details">~2-hour scenic drive</div>
                </div>
            </div>
            
            <div class="hotel-info">
                <div class="hotel-name">Happy Cretan Suites</div>
                <div>Marikas Kapsi, Agia Pelagia • 4 nights</div>
                <div>Confirmation: <span class="confirmation-code">72954215794020</span></div>
            </div>
            
            <div class="reservation-highlight">
                <strong>Dinner: Erganos</strong><br>
                Traditional Cretan cuisine (contacted via Facebook)
            </div>
        </div>
    </div>
    <!-- HERAKLION DAYS -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 7 - Choose Your Adventure</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">HERAKLION - Day 2</span>
            
            <div class="contact-info">
                <strong>Choose One Adventure:</strong>
            </div>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-title">Option 1: Sea Kayaking</div>
                    <div class="activity-details">Enjoy Crete tour - paddle coastline, explore caves, swim/snorkel, lunch in Agia Pelagia</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-title">Option 2: Historical Sites</div>
                    <div class="activity-details">Knossos Palace & Archaeological Museum (book advance tickets), Koules Fortress, lunch at Kouzina</div>
                </div>
                
                <div class="activity-card">
                    <div class="activity-title">Option 3: Wine Tasting</div>
                    <div class="activity-details">Douloufakis or Lyrarakis Winery, vineyard views, winery lunch</div>
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>7:00 PM - Dinner Reservation</strong><br>
                <strong>Peskesi</strong>
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 8 - Catamaran Adventure</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">HERAKLION - Day 3</span>
            
            <div class="reservation-highlight">
                <strong>Full Day - Semi-Private Catamaran Cruise</strong><br>
                <strong>Green Cruises or DanEri Yachts</strong><br>
                • Dia Island or Heraklion coast<br>
                • Swimming & snorkeling<br>
                • Onboard meal/brunch included
            </div>
            
            <div class="reservation-highlight">
                <strong>8:00 PM - Dinner Reservation</strong><br>
                <strong>7 Thalasses</strong>
            </div>
        </div>
    </div>
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 9 - Relaxation Day</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">HERAKLION - Day 4</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">All Day</div>
                    <div class="activity-title">Beach Relaxation</div>
                    <div class="activity-details">Chill at Agia Pelagia Beach or Ammoudara Beach near Heraklion</div>
                </div>
            </div>
            
            <div class="contact-info">
                <strong>Farewell Dinner Options:</strong><br>
                • Kastella (seaside seafood)<br>
                • Parasties (traditional open-flame Cretan food)<br>
                • Herb's Garden (rooftop with harbor views)
            </div>
        </div>
    </div>
    <!-- DEPARTURE -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>October 10 - Departure Day</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <span class="location-badge">DEPARTURE</span>
            
            <div class="activity-grid">
                <div class="activity-card">
                    <div class="activity-time">Morning</div>
                    <div class="activity-title">Farewell Brunch</div>
                    <div class="activity-details">Sea view brunch at Opus Wine Bar or Phyllo Sophies</div>
                </div>
            </div>
            
            <div class="flight-info">
                <div class="activity-title">Return Flight HER → BOS</div>
                <div><strong>Departure:</strong> 2:40 PM from Heraklion</div>
                <div><strong>Arrival:</strong> 10:40 PM in Boston (same day)</div>
                <div><strong>Airlines:</strong> British Airways & American Airlines</div>
                <div><strong>Flights:</strong> BA 743 → AA 6982 (London layover)</div>
                <div><strong>Confirmation:</strong> <span class="confirmation-code">3ZMLX5</span></div>
            </div>
            
            <div class="contact-info">
                <strong>Car Return:</strong> Europcar at Heraklion Airport before departure
            </div>
        </div>
    </div>
    <!-- QUICK REFERENCE -->
    <div class="day-section">
        <div class="day-header" onclick="toggleDay(this)">
            <h2>Quick Reference - Important Info</h2>
            <span class="toggle-arrow">+</span>
        </div>
        <div class="day-content">
            <div class="emergency-contacts">
                <div class="contact-info">
                    <strong>Travel Agent</strong><br>
                    Lori Oliveira - FORA<br>
                    lori.oliveira@fora.travel
                </div>
                
                <div class="contact-info">
                    <strong>Expedia Support</strong><br>
                    TAAP: +1 (866) 925-7718<br>
                    (For hotel bookings)
                </div>
                
                <div class="contact-info">
                    <strong>Flight Confirmations</strong><br>
                    Outbound: GUUKWU<br>
                    Return: 3ZMLX5<br>
                    Ferry: 1112EKUZN
                </div>
                
                <div class="contact-info">
                    <strong>Car Rental</strong><br>
                    Europcar<br>
                    Conf: 73062353442813<br>
                    Pickup: Chania Oct 3<br>
                    Return: Heraklion Oct 10
                </div>
            </div>
            
            <div class="reservation-highlight">
                <strong>Still Need to Book:</strong><br>
                • Knossos Palace tickets (advance booking required)<br>
                • Rhina Naxos Kayaking<br>
                • Sea Kayaking Crete tour<br>
                • Spa treatments in Chania/Heraklion<br>
                • Final restaurant confirmations
            </div>
        </div>
    </div>
    <div class="footer">
        <h2>Have an Amazing Honeymoon!</h2>
        <p>This itinerary is your guide - feel free to be spontaneous and adjust as you go. The most important thing is to enjoy each other's company and create beautiful memories together in Greece.</p>
        
        <div style="margin-top: 20px; font-style: italic; color: #666;">
            Curated by Lori Oliveira - FORA Travel<br>
            Safe travels, Justin & Shay!
        </div>
    </div>
</div>
<script>
    function toggleDay(header) {
        const content = header.nextElementSibling;
        const arrow = header.querySelector('.toggle-arrow');
        
        if (content.classList.contains('active')) {
            content.classList.remove('active');
            arrow.textContent = '+';
            arrow.style.transform = 'rotate(0deg)';
        } else {
            content.classList.add('active');
            arrow.textContent = '−';
            arrow.style.transform = 'rotate(180deg)';
        }
    }
    
    // Auto-expand current day
    const today = new Date();
    const tripStart = new Date('2025-09-26');
    const daysDiff = Math.ceil((today - tripStart) / (1000 * 60 * 60 * 24));
    
    if (daysDiff >= 0 && daysDiff < 15) {
        const daySections = document.querySelectorAll('.day-section');
        if (daySections[daysDiff]) {
            const header = daySections[daysDiff].querySelector('.day-header');
            toggleDay(header);
        }
    }
</script>
</body> </html>

