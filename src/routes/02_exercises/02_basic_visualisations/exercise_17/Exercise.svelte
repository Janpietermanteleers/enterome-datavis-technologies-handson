

<script>

    import{scaleLinear} from 'd3-scale'
    // Dimensions
    const width = 800;
    const height = 100;
    const scale = scaleLinear().domain([0, height]).range([0, width]);
    const margin = { top: 5, right: 5, bottom: 5, left: 5 };
    const innerWidth = width - margin.left - margin.right;
    const innerHeight = height - margin.top - margin.bottom;
  
    // Array
    const values = [2, 4, 6, 7, 9];
  </script>
  
  <svg viewBox="0 0 {width} {height}">
    <g transform="translate({margin.left},{margin.top})">
      <circle cx="{scale(values[0])}"   cy="{innerHeight/2}"   r="10" />
      <circle cx="{scale(values[1])}" cy="{innerHeight/2}"   r="10" />
      <circle cx="{scale(values[2])}"   cy="{innerHeight/2}"  r="10" />
      <circle cx="{scale(values[3])}"  cy="{innerHeight/2}"   r="10" />
      <circle cx="{scale(values[4])}"   cy="{innerHeight/2}" r="10" />
    </g>
  </svg>
  