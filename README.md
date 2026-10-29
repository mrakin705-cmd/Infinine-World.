# Infinine-World.
A infinine build and adventrure 2D building world
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>—Blockscape 2D Sandbox</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <main id="homeScreen" class="screen home-screen">
      <div class="home-card">
        <div class="logo-mark" aria-hidden="true">0</div>
        <p class="eyebrow">Build anything you like</p>
        <h1>Infinine World</h1>
        <p class="intro">Build anything you can imagine, one block at a time.</p>
        <div class="preview-blocks" aria-hidden="true">
          <span class="block wood"></span><span class="block stone"></span>
          <span class=""></span><span class=""></span>
        </div>
        <div class="mode-options" role="group" aria-label="Choose a game mode">
          <button class="mode-option selected" data-mode="survival" aria-pressed="true">
            <strong>Survival</strong><span>Explore the world</span>
          </button>
           that one is coming soon
              ......<===== try that
          
          </button>
        </div>
        <button id="playButton" class="primary-button">Play now <span>→</span></button>
        <p class="home-hint">A infinine build and adventrure 2D building world</p>
      </div>
    </main>

    <main id="gameScreen" class="screen game-screen hidden">
      <header class="topbar">
        <button id="homeButton" class="icon-button" aria-label="Back to home">←</button>
        <div class="game-brand"><span class="mini-logo">▦</span><strong>Blockscape</strong></div>
        <div class="world-label"><span class="live-dot"></span> Creative world</div>
        <div id="healthHud" class="health-hud hidden" aria-label="Health"><span>♥</span><div class="health-track"><i id="healthFill"></i></div><strong id="healthText">100</strong></div>
        <button id="inventoryButton" class="inventory-button hidden">Inventory <kbd>E</kbd></button>
        <button id="aiButton" class="ai-button"><span>✦</span> AI Builder</button>
      </header>
      <section class="game-area">
        <canvas id="world" aria-label="Block building world"></canvas>
        <div class="tip-card" id="tipCard">
          <button id="closeTip" aria-label="Dismiss tips">×</button>
          <strong>Your world, your rules</strong>
          <span>Click to build · Right-click to erase</span>
          <span>A / D move · W / Space jump · S fall faster</span>
        </div>
        <div class="toast" id="toast" role="status"></div>
        <section id="inventoryPanel" class="inventory-panel hidden" aria-label="Inventory and crafting">
          <button id="closeInventory" class="inventory-close" aria-label="Close inventory">×</button>
          <h2>Inventory &amp; crafting</h2>
          <p class="inventory-instructions">Click a tree three times (once with an axe) to collect logs. Craft a table first to unlock tools; use a pickaxe to mine nearby dirt and stone.</p>
          <div id="inventoryItems" class="inventory-items"></div>
          <div class="crafting-recipes">
            <button class="recipe-button" data-recipe="table">Crafting table <span>4 logs</span></button>
            <button class="recipe-button" data-recipe="axe">Wooden axe <span>3 logs + table</span></button>
            <button class="recipe-button" data-recipe="pickaxe">Wooden pickaxe <span>3 logs + table</span></button>
          </div>
        </section>
        <div class="hotbar" role="group" aria-label="Inventory hotbar">
          <button class="material hotbar-slot selected" data-material="wood" data-slot="1" title="Wood (1)" aria-label="Select wood">
            <span class="swatch wood"></span><span class="slot-count" data-count="wood">∞</span><kbd>1</kbd>
          </button>
          <button class="material hotbar-slot" data-material="stone" data-slot="2" title="Stone (2)" aria-label="Select stone">
            <span class="swatch stone"></span><span class="slot-count" data-count="stone">∞</span><kbd>2</kbd>
          </button>
          <button class="material hotbar-slot" data-material="glass" data-slot="3" title="Glass (3)" aria-label="Select glass">
            <span class="swatch glass"></span><span class="slot-count" data-count="glass">∞</span><kbd>3</kbd>
          </button>
          <button class="material hotbar-slot" data-material="dirt" data-slot="4" title="Dirt (4)" aria-label="Select dirt">
            <span class="swatch dirt"></span><span class="slot-count" data-count="dirt">∞</span><kbd>4</kbd>
          </button>
          <button id="inventorySlot5" class="empty-slot tool-slot" data-slot="5" aria-label="Empty inventory slot 5"><kbd>5</kbd></button>
          <button id="inventorySlot6" class="empty-slot tool-slot" data-slot="6" aria-label="Empty inventory slot 6"><kbd>6</kbd></button>
          <button id="inventorySlot7" class="empty-slot tool-slot" data-slot="7" aria-label="Empty inventory slot 7"><kbd>7</kbd></button>
          <button class="empty-slot" data-slot="8" aria-label="Empty inventory slot 8"><kbd>8</kbd></button>
          <button class="empty-slot" data-slot="9" aria-label="Empty inventory slot 9"><kbd>9</kbd></button>
        </div>
        <div class="move-hint"><span>↔</span> A / D move · W jump · S faster fall · Right-click erase</div>
        <div class="world-version">Infinite World v1.0</div>
      </section>
    </main>
    <script src="script.js"></script>
  </body>
</html>
