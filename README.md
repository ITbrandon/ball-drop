## Ball Drop Game

### Variables and Sprites:
- Set player speed to 1
- Set player lives to 3
- Set player score to 0
- Set ball speed to -5
- Set player position to bottom center of screen
- Set ball position to top of screen

### Game Loop:
while game is running:
    // Handle user input
    if a key pressed:
        Move player left
    Else if d key pressed:
        Move player right
        
    // Update game state
    Update player position
    Check for collisions with balls
    Update player score
        
    // Render game
    Show player sprite
    Show falling ball sprites
    Show player score
    Show player lives
    hide ball speed
        
    // Check for game over conditions
    if player loses all lives:
        Set game over
        Show game over message
        Stop game loop
              
    // Increment ball speed by small amount every time Ball hits Ground
        
    // Control the dropping balls
    For each ball:
        if ball reaches ground:
            Reset ball position to top of screen
            Increment player score
            Increment player speed
        else if ball touches player:
            Decrement player lives
            Reset ball position to top of screen
            If player loses all lives:
                Set game over
                Show game over message
                Stop game loop

### Custom Block:
- CheckCollision (takes input: ball sprite)
    - Check if ball sprite touches player sprite