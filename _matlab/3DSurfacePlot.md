  <details>
    <summary>三維曲面圖</summary>
    
```cpp
  [x, y] = meshgrid(-3:0.1:3, -3:0.1:3);
  z = sin(x) + cos(y);
  figure;
  surf(x, y, z);
  title(‘三維曲面圖: z = sin(x) + cos(y)');
  xlabel('X軸');
  ylabel('Y軸');
  zlabel('Z軸');
  colorbar;
  shading interp; % 平滑著色
```

</details>

![三維曲面圖](三維曲面圖.png)
  
