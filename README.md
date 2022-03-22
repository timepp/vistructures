# vistructures: A structured data visualizer

> contents comming soon

## introduction

`vistructures` shows a web GUI to visualize arbitrary data which meets the following loose requirements:

1. The data is given by a json file
2. It's an array with items that has similar structure

Each item is shown as a tile or table row. Each tile can have an image (specified by your configuration), if there is no image then the tile will be colored based on item name. You can filter items based on there properties. Each item has a detailed page, from where a dynamic set of gallery images can be shown. You can define the action when an item is clicked.

## usage

### prerequisites

- deno (<https://deno.land>)

### run the demo

```bash
deno run -A server.ts config_sample.ts 
```

### visualize you own data

1. copy `config_sample.ts` to `config.ts` and make your customizations. See comments inside this file.
2. run:

    ```bash
    deno run -A server.ts config.ts
    ```

    this will start a local http server and open your default browser to show your data in the way you specified in `config.ts`.
