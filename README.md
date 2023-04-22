# understand-helix

for link in `https://helix-editor.com/`

toBeOnDisk => links above
1. to!BeOnDisk => remove .cach .config ...
2. N helixOnDisk? => not necessary

toBeOnMemo => `h`, `hx`
1. to!BeOnMemo:
    1. abbr&whole => :q, :quit
    2. + remove changes => :q!
    3. + save changes, so remove origin file => :wq, :wqa(diff on number)
2. N helixOnMemo? => not necessary

TEXT => toBeOnDisk => `hx a.txt, :w`, `touch`
1. to!Be => `rm a.txt`
2. N toBeOnDisk => `cp`

TEXT => toBeOnMemo => `hx a.txt`
1. to!Be => `:q!`, ?

toBeBetter
1. add to initSctip: alias h='hx'
2. reset keymap based on my own conditions and needs

models
1. 1D char[]: dimension{x} x 2 directions{f/b} x step{char, word, sentence, paragraph, fn, {}block, etc...}, two ENDS.
    1. w => forward to word's end, contains a space after word if exist&through
    2. e => forward to word's end, contains a space before word if exist&through
    3. how to select whole word?
        1. ebd or bed
        2. mawd
        3. daw from vim???
    4. W, 2w, 8l, 8h, with relative ruler
2. 2D char[][]: 2 dimensions{x/y} x 2 directions{f/b}, four directions, four ENDS, (x, y).
    1. is bigger than screen[][], so drag logical BIG text around the screen.
    2. and there is another dragging => drag cursor.
3. 2D char[][] visible:
4. screen[][] cells:
5. window[][] cells: some warning msg;
5. combinations, mixture of models
    1. `h` has two forms by default:
        1. 1D char[][] => b by a char
        2. 2D char[][] => b by a char in dimensionX
            1. There for `gh` => leftmost

file/directory
1. create
2. r/w
2. delte

cmd, shell i/o

cursor, selection, text, window

selection
1. one of position[]? => cursor
    1. toBeOnScreen? => Nope, default is 1 cell cursor-main-selection.
    2. to!BeOnScreen? => Nope, why?
2. N positions => selection

multi-selections?
1. multi positions selectable
2. multi levels: selections' selection
3. multi prority: cursor/selection
