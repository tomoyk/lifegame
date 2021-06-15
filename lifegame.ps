int box_size = 20;
int box_count = 40;
boolean[][] cells = new boolean[box_count][box_count];

void setup() {
  // box_size * box_count
  size(800, 800);

  // x, y
  cells[2][2] = true;
  cells[3][2] = true;
  cells[4][2] = true;
  cells[2][3] = true;
  cells[3][4] = true;

  // Random true set
  for (int p=0; p<box_size; p++) {
    int x1 = (int)random(box_count);
    int y1 = (int)random(box_count);
    for (int q=0; q<10; q++) {
      try {
        int a1 = (int)random(-3, 3); // -2, -1, 0, 1, 2
        int a2 = (int)random(-3, 3); // -2, -1, 0, 1, 2
        cells[x1+a1][y1-a2] = true;
      }
      catch (ArrayIndexOutOfBoundsException e) {
        continue;
      }
    }
  }

  // Rendering
  for (int y=0; y<box_count; y++) {
    for (int x=0; x<box_count; x++) {
      if (false == cells[x][y]) {
        fill(255); // white
      } else {
        fill(0); // black
      }
      rect(x*box_size, y*box_size, box_size, box_size);
    }
  }
}

// live=1 death=0
boolean judge(boolean[][] cells, int center_x, int center_y) {
  int total_alive = 0;
  for (int x=-1; x<=1; x++) {
    for (int y=-1; y<=1; y++) {
      try {
        if (x == 0 && y == 0) {
          continue;
        }
        if (true == cells[center_x+x][center_y+y]) {
          total_alive += 1;
        }
      } 
      catch (ArrayIndexOutOfBoundsException e) {
        continue;
      }
    }
  }
  // println("total_alive=", total_alive);

  boolean is_alive = cells[center_x][center_y];
  if (false == is_alive && total_alive == 3) {
    return true;
  } else if (true == is_alive && (total_alive == 2 || total_alive == 3)) {
    return true;
  } else if (true == is_alive && total_alive <= 1) {
    return false;
  } else if (true == is_alive && total_alive >= 4) {
    return false;
  }

  return false;
}

void draw() {
  // if (mousePressed == true) {
  delay(100);

  // Initialize memo vars
  int memo_len = box_count*box_count;
  int[] memo_x = new int[memo_len];
  int[] memo_y = new int[memo_len];
  int memo_index = 0;
  for (int i=0; i<memo_len; i++) {
    memo_x[i] = -1;
    memo_y[i] = -1;
  }

  // Rendering cells and Determining next cell value
  for (int y=0; y<box_count; y++) {
    for (int x=0; x<box_count; x++) {
      if (false == cells[x][y]) {
        fill(255); // white
      } else {
        fill(0); // black
      }
      rect(x*box_size, y*box_size, box_size, box_size);

      boolean next_alive = judge(cells, x, y);
      if (next_alive != cells[x][y]) {
        println("update: cells[", x, "][", y, "] : ", cells[x][y], "->", next_alive);
        // cells[x][y] = next_alive;
        memo_x[memo_index] = x;
        memo_y[memo_index] = y;
        memo_index++;
      }
    }
  }

  // Update cell values
  for (int i=0; i<memo_len; i++) {
    if (memo_x[i] == -1 || memo_y[i] == -1) {
      break;
    }
    cells[memo_x[i]][memo_y[i]] = !cells[memo_x[i]][memo_y[i]];
  }
  // }

  /* Debug
   for(int i=0; i<cells.length; i++){
   for(int j=0; j<cells[i].length; j++) {
   print(cells[i][j], " ");
   }
   println();
   }
   */
}
