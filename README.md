# Supabase-FramerConnector
A connection component for Framer and Supabase

## Requirements

- Use in Framer Web or Framer Desktop
- It needs access to a centralized `store` object in order to save the supabase client instance

A file like `globals.ts` with the below syntax is enough
```
import { createStore } from "https://framer.com/m/framer/store.js@^1.0.0"

export const globalStore = createStore({
  supabase:null
})
```
The `SupabaseConnector` will pick it up then automatically


## Use

Drag and drop the component from the `Code` bar on your Framer project into the canvas (make sure that the View that contains the `SupabaseConnector` will run before any Supabase operations are invoked)

## Notes

The component also allows the saving of up to six database names to be used as global store variables (an ease of use feature mostly)
