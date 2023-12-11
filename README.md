# VerilogPong

![Menu Screenshot](https://github.com/vtneil/VerilogPong/blob/master/screenshots/01_Menu.png?raw=true)

An FPGA-based Pong game with some twists written in Verilog HDL. This game has two pongs (balls). The paddles can be moved in both X and Y direction. The game will end if either player has scored 21 or more. It also features a "dealbreaker" scoring which the player has to score 2 more balls than another player to win.

## Designs

It is very modular with Graphics Processer, ASCII String Renderer, Pixel Overlay using Priority Multiplexing, VGA, PS/2 Keyboard, UART Controller, Hierarchical Finite State Machine, Graphics Context Manager, etc.

The game is controlled by a Hierarchical FSM with global states (Top-level) and game states (Hierarchical level).

## Controls

The game is controlled by USB keyboard (via PS/2 protocol).
1. [SPACE] for accept/continue
2. [W], [A], [S], [D] for Player 1's paddle
3. [I], [J], [K], [L] for Player 2's paddle
4. [ESC] for game reset
5. [F5] for VGA reset

## Other Notes

* Note: this game is a final project for 2110363 (Hardware Synthesis Laboratory I) of 1/2023.
* The game is tested on Basys 3 board.