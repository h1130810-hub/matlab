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

 <details>
    <summary>三維網格圖</summary>
   
```cpp
  [x, y] = meshgrid(-2:0.2:2);
  z = x .* exp(-x.^2 - y.^2);
  figure;
  mesh(x, y, z);
  title('三維網格圖: z = x * exp(-x² - y²)');
  xlabel('X軸');
  ylabel('Y軸');
  zlabel('Z軸');
  colormap(jet);
```

</details>

![三維曲面圖](三維網格圖.png)
