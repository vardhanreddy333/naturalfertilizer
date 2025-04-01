<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Natural Fertilizer Production</title>
    <style>
        :root {
            --primary: #4a8f29;
            --secondary: #e8f5e9;
            --accent: #ff9800;
            --dark: #2e7d32;
            --light: #f1f8e9;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        nav {
            background-color: var(--dark);
            padding: 0.5rem 0;
        }
        
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            flex-wrap: wrap;
        }
        
        nav ul li {
            margin: 0 10px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            padding: 5px 10px;
            border-radius: 4px;
            transition: background-color 0.3s;
        }
        
        nav ul li a:hover, nav ul li a.active {
            background-color: var(--accent);
        }
        
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1605000797499-95a51c5269ae');
            background-size: cover;
            background-position: center;
            height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .content-section {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        
        .content-section h2 {
            color: var(--primary);
            margin-bottom: 1rem;
            border-bottom: 2px solid var(--secondary);
            padding-bottom: 0.5rem;
        }
        
        .fertilizer-card {
            background-color: var(--secondary);
            border-left: 4px solid var(--primary);
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border-radius: 0 4px 4px 0;
        }
        
        .fertilizer-card h3 {
            color: var(--dark);
            margin-bottom: 0.5rem;
        }
        
        .fertilizer-card h4 {
            margin: 1rem 0 0.5rem;
            color: var(--primary);
        }
        
        .fertilizer-card ul {
            margin-left: 1.5rem;
        }
        
        .fertilizer-card p {
            margin-bottom: 0.5rem;
        }
        
        .comparison-table {
            width: 100%;
            border-collapse: collapse;
            margin: 1rem 0;
        }
        
        .comparison-table th, .comparison-table td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        
        .comparison-table th {
            background-color: var(--primary);
            color: white;
        }
        
        .comparison-table tr:nth-child(even) {
            background-color: var(--secondary);
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 8px 16px;
            border-radius: 4px;
            text-decoration: none;
            margin-top: 1rem;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #f57c00;
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 5px 0;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Natural Fertilizer Production</h1>
            <p>Sustainable Solutions for Soil Health</p>
        </div>
    </header>
    
    <nav>
        <div class="container">
            <ul>
                <li><a href="#" class="active" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('fertilizers')">Fertilizer Types</a></li>
                <li><a href="#" onclick="showSection('importance')">Why Natural?</a></li>
                <li><a href="#" onclick="showSection('comparison')">Food Waste Conversion</a></li>
            </ul>
        </div>
    </nav>
    
    <div class="container">
        <section id="home-section">
            <div class="hero">
                <div>
                    <h1>Transform Waste into Garden Gold</h1>
                    <p>Learn how to create natural fertilizers from household and agricultural waste</p>
                </div>
            </div>
            
            <div class="content-section">
                <h2>Welcome to Natural Fertilizer Production</h2>
                <p>Our mission is to promote sustainable agriculture through the use of natural fertilizers made from organic waste materials. By converting food scraps, yard waste, and other biodegradable materials into nutrient-rich soil amendments, we can:</p>
                <ul>
                    <li>Reduce landfill waste</li>
                    <li>Improve soil health</li>
                    <li>Increase crop yields naturally</li>
                    <li>Protect water quality</li>
                    <li>Combat climate change</li>
                </ul>
                <p>Explore our resources to learn about different natural fertilizer production methods and their benefits for your garden or farm.</p>
            </div>
        </section>
        
        <section id="fertilizers-section" style="display: none;">
            <div class="content-section">
                <h2>Natural Fertilizer Types</h2>
                <p>Discover various methods to create natural fertilizers from organic materials:</p>
                
                <div class="fertilizer-card">
                    <h3>Compost</h3>
                    <h4>Primary Ingredients:</h4>
                    <p>Food waste (vegetable peels, fruit scraps, coffee grounds), yard waste, manure, leaves, grass clippings</p>
                    
                    <h4>Detailed Preparation:</h4>
                    <p><strong>FOOD WASTE CONVERSION PROCESS:</strong><br>
                    1. Collection: Separate biodegradable food waste from non-compostables<br>
                    2. Preparation: Chop larger pieces to speed decomposition<br>
                    3. Layering: Alternate food waste (green material) with brown material (dry leaves, paper) in 1:3 ratio<br>
                    4. Moisture Control: Maintain 40-60% moisture (like a wrung-out sponge)<br>
                    5. Aeration: Turn pile weekly to introduce oxygen<br>
                    6. Temperature Monitoring: Ideal range 135-160°F for pathogen kill<br>
                    7. Maturation: Allow 2-12 months for complete decomposition</p>
                    
                    <p><strong>SCIENTIFIC NOTES:</strong><br>
                    - Microbial activity breaks down complex organics into humus<br>
                    - Carbon:Nitrogen ratio critical (25-30:1 ideal)<br>
                    - Thermophilic phase kills pathogens and weed seeds</p>
                    
                    <h4>Proven Benefits:</h4>
                    <ul>
                        <li>Improves soil structure by increasing porosity</li>
                        <li>Enhances water retention by 20-40% in sandy soils</li>
                        <li>Provides balanced NPK (typically 1-1-1) plus micronutrients</li>
                        <li>Suppresses plant diseases through competitive exclusion</li>
                        <li>Reduces landfill waste by diverting food scraps</li>
                    </ul>
                    
                    <h4>Recommended Application:</h4>
                    <p>Vegetable gardens: 2-4 inches worked into top 6" of soil<br>
                    Lawns: 1/4-1/2 inch top dressing<br>
                    Trees: 3" mulch ring (keep away from trunk)</p>
                    
                    <h4>Scientific Background:</h4>
                    <p>Composting mimics natural decomposition but accelerates it through controlled conditions. Bacteria (especially thermophiles like Bacillus spp.) and fungi (Aspergillus, Trichoderma) break down organic matter. The process converts nitrogen from unstable ammonia forms to stable organic compounds, preventing leaching while making nutrients plant-available.</p>
                </div>
                
                <div class="fertilizer-card">
                    <h3>Vermicompost (Worm Castings)</h3>
                    <h4>Primary Ingredients:</h4>
                    <p>Food waste (no meat/dairy), cardboard, paper, coconut coir, red wigglers (Eisenia fetida)</p>
                    
                    <h4>Detailed Preparation:</h4>
                    <p><strong>STEP-BY-STEP VERMICOMPOSTING:</strong><br>
                    1. Bin Setup: Drill ventilation holes in plastic container (10-12" deep)<br>
                    2. Bedding: Soak shredded newspaper/cardboard to 75% moisture<br>
                    3. Worm Introduction: Add 1 lb worms per 1/2 lb daily food waste<br>
                    4. Feeding: Bury food waste in different zones each time<br>
                    5. Maintenance: Keep pH 6-8, temp 55-77°F<br>
                    6. Harvesting: After 3-6 months, use light to drive worms from finished castings</p>
                    
                    <p><strong>FOOD WASTE TIPS:</strong><br>
                    - Best: Fruit/veggie scraps, coffee grounds, crushed eggshells<br>
                    - Avoid: Citrus, onions, meat, oily foods<br>
                    - Particle size &lt;1" speeds processing</p>
                    
                    <h4>Proven Benefits:</h4>
                    <ul>
                        <li>5-11 times more nutrients than regular compost</li>
                        <li>Contains plant growth hormones (auxins, cytokinins)</li>
                        <li>Improves seed germination and plant growth rates</li>
                        <li>Suppresses diseases (contains chitinase-producing bacteria)</li>
                        <li>Can be made indoors year-round</li>
                    </ul>
                    
                    <h4>Recommended Application:</h4>
                    <p>Seed starting: Mix 10-20% with potting medium<br>
                    Transplants: 1/4 cup in planting hole<br>
                    Top dressing: 1/2" around plants every 2 months</p>
                    
                    <h4>Scientific Background:</h4>
                    <p>Earthworms digest organic matter with help from gut microbes, producing castings with higher nutrient availability than compost. The process increases surface area for microbial colonization and stabilizes nutrients in humic compounds. Worm mucus (coelomic fluid) acts as a natural chelator, making minerals more plant-available.</p>
                </div>
                
                <div class="fertilizer-card">
                    <h3>Bokashi (Fermented Food Waste)</h3>
                    <h4>Primary Ingredients:</h4>
                    <p>All food waste (including meat/dairy), bran, molasses, EM (Effective Microorganisms)</p>
                    
                    <h4>Detailed Preparation:</h4>
                    <p><strong>BOKASHI FERMENTATION PROCESS:</strong><br>
                    1. Inoculate bran with EM solution (1 tbsp EM + 1 tbsp molasses per cup water)<br>
                    2. Layer food waste in airtight bucket, sprinkling bran between layers<br>
                    3. Compress to remove air pockets<br>
                    4. Drain liquid weekly (use diluted 100:1 as fertilizer)<br>
                    5. After 2-4 weeks, material is fermented (not decomposed)<br>
                    6. Bury in soil trenches or add to compost pile to finish</p>
                    
                    <p><strong>KEY DIFFERENCES FROM COMPOSTING:</strong><br>
                    - Works anaerobically (no turning needed)<br>
                    - Ferments rather than decomposes<br>
                    - Handles all food waste including meats<br>
                    - Process is much faster (2 weeks vs months)</p>
                    
                    <h4>Proven Benefits:</h4>
                    <ul>
                        <li>Preserves 100% of nutrient content (no loss to air/heat)</li>
                        <li>Lactic acid suppresses pathogens</li>
                        <li>Can process meat, dairy, and cooked foods safely</li>
                        <li>Produces nutrient-rich leachate for liquid feeding</li>
                        <li>Works in small spaces (apartment-friendly)</li>
                    </ul>
                    
                    <h4>Recommended Application:</h4>
                    <p>Pre-planting: Bury 6-8" deep 2 weeks before planting<br>
                    Existing plants: Bury around drip line<br>
                    Pot plants: Mix 1:10 with soil</p>
                    
                    <h4>Scientific Background:</h4>
                    <p>Bokashi relies on lacto-fermentation by anaerobic bacteria (Lactobacillus spp.) and yeasts. The acidic environment (pH ~4) preserves nutrients while breaking down complex molecules. After burial, aerobic soil microbes rapidly complete decomposition. This two-phase process minimizes greenhouse gas emissions compared to traditional composting.</p>
                </div>
            </div>
        </section>
        
        <section id="importance-section" style="display: none;">
            <div class="content-section">
                <h2>Scientific & Environmental Importance of Natural Fertilizers</h2>
                
                <h3>1. SOIL HEALTH RESTORATION:</h3>
                <ul>
                    <li>Increases organic matter by 1-3% annually (USDA recommends 5% ideal)</li>
                    <li>Improves cation exchange capacity (CEC) by 20-50%, enhancing nutrient retention</li>
                    <li>Boosts microbial biomass by 2-10x compared to synthetic fertilizer use</li>
                </ul>
                
                <h3>2. CLIMATE CHANGE MITIGATION:</h3>
                <ul>
                    <li>Sequesters 0.5-2 tons carbon/acre/year in stable humus forms</li>
                    <li>Reduces N2O emissions by 40-70% compared to synthetic nitrogen</li>
                    <li>Eliminates fossil fuel use in fertilizer production (1kg N fertilizer = 1.5kg oil equivalent)</li>
                </ul>
                
                <h3>3. WATER QUALITY PROTECTION:</h3>
                <ul>
                    <li>Reduces nitrate leaching by 60-90% compared to chemical fertilizers</li>
                    <li>Prevents algal blooms by minimizing phosphorus runoff</li>
                    <li>Improves water infiltration rates by 30-50% in compacted soils</li>
                </ul>
                
                <h3>4. BIODIVERSITY SUPPORT:</h3>
                <ul>
                    <li>Increases earthworm populations by 300-500%</li>
                    <li>Supports mycorrhizal fungi networks (increase root absorption area 100x)</li>
                    <li>Maintains soil microarthropod diversity critical for decomposition</li>
                </ul>
                
                <h3>5. ECONOMIC BENEFITS:</h3>
                <ul>
                    <li>Saves $50-200/acre/year on fertilizer costs (Rodale Institute data)</li>
                    <li>Increases yields by 10-30% over 5-7 years as soil health improves</li>
                    <li>Reduces irrigation needs by 20-40% through better water retention</li>
                </ul>
                
                <h3>6. FOOD QUALITY IMPROVEMENT:</h3>
                <ul>
                    <li>Increases antioxidant levels in crops by 15-40% (JAS study data)</li>
                    <li>Enhances vitamin and mineral content through balanced nutrition</li>
                    <li>Reduces pesticide residues by promoting plant immune systems</li>
                </ul>
            </div>
        </section>
        
        <section id="comparison-section" style="display: none;">
            <div class="content-section">
                <h2>Food Waste to Fertilizer: Comparative Methods</h2>
                
                <table class="comparison-table">
                    <tr>
                        <th>Method</th>
                        <th>Processing Time</th>
                        <th>Inputs</th>
                        <th>Output</th>
                        <th>Nutrient Retention</th>
                        <th>Carbon Footprint</th>
                        <th>Best For</th>
                    </tr>
                    <tr>
                        <td>Traditional Composting</td>
                        <td>2-12 months</td>
                        <td>Fruit/veggie scraps, yard waste</td>
                        <td>50-70% volume reduction</td>
                        <td>60-80% N, 70-90% P/K</td>
                        <td>0.05kg CO2/kg waste</td>
                        <td>Yard-scale operations, bulk processing</td>
                    </tr>
                    <tr>
                        <td>Vermicomposting</td>
                        <td>3-6 months</td>
                        <td>All food waste except citrus/onions</td>
                        <td>10-20% original volume as castings</td>
                        <td>90-95% N, 85% P/K</td>
                        <td>0.02kg CO2/kg waste</td>
                        <td>Urban settings, high-value fertilizer production</td>
                    </tr>
                    <tr>
                        <td>Bokashi Fermentation</td>
                        <td>2-4 weeks (plus 2 week soil finish)</td>
                        <td>ALL food waste including meat/dairy</td>
                        <td>Minimal volume reduction</td>
                        <td>98-100% of all nutrients</td>
                        <td>0.01kg CO2/kg waste</td>
                        <td>Apartments, meat-eating households</td>
                    </tr>
                    <tr>
                        <td>Black Soldier Fly Larvae</td>
                        <td>2-3 weeks</td>
                        <td>High-nutrient waste (meat, dairy, grains)</td>
                        <td>10% frass, 15% larvae (for animal feed)</td>
                        <td>80% N in frass</td>
                        <td>0.03kg CO2/kg waste</td>
                        <td>Commercial-scale operations, integrated farming</td>
                    </tr>
                </table>
                
                <h3>Choosing the Right Method:</h3>
                <p>Selecting the best food waste conversion method depends on several factors:</p>
                <ul>
                    <li><strong>Space available:</strong> Bokashi and vermicomposting work well in small spaces, while traditional composting requires more area</li>
                    <li><strong>Types of waste:</strong> Households with meat/dairy waste should consider bokashi or black soldier fly systems</li>
                    <li><strong>Time constraints:</strong> Bokashi is fastest, while traditional composting takes longest</li>
                    <li><strong>End use:</strong> Vermicompost produces the highest-value fertilizer, while black soldier fly systems also produce animal feed</li>
                </ul>
            </div>
        </section>
    </div>
    
    <footer>
        <div class="container">
            <p>&copy; 2023 Natural Fertilizer Production | Sustainable Agriculture Solutions</p>
            <p>Contact: info@naturalfertilizers.org | (123) 456-7890</p>
        </div>
    </footer>
    
    <script>
        function showSection(sectionId) {
            // Hide all sections
            document.getElementById('home-section').style.display = 'none';
            document.getElementById('fertilizers-section').style.display = 'none';
            document.getElementById('importance-section').style.display = 'none';
            document.getElementById('comparison-section').style.display = 'none';
            
            // Show selected section
            document.getElementById(sectionId + '-section').style.display = 'block';
            
            // Update active nav link
            const navLinks = document.querySelectorAll('nav ul li a');
            navLinks.forEach(link => {
                link.classList.remove('active');
            });
            event.target.classList.add('active');
        }
    </script>
</body>
</html>
