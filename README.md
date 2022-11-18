# SkillChains
### Active Battle Skillchain Display.

Enhanced to allow automatic skill chaining based on the current skill chain and available weaponskills. The auto weaponskill addon will react to weaponskills done by other players.

Displays a text object containing skillchain elements resonating on current target, timer for skillchain window,
along with a list of weapon skills that can skillchain based on the weapon you have currently equipped. 

    //sc color    -- colorize properties and elements
    
    //sc move     -- displays text box click and drag it to desired location.

    //sc save     -- save settings to current character.

    //sc save all -- save settings to all characters.

The following commands toggle the display information and are saved on a per job basis.

    //sc spell    -- sch immanence and blue magic spells.

    //sc pet      -- smn and bst pet skills.

    //sc weapon   -- weapon skills.

    //sc burst    -- magic burst elements.

    //sc props    -- skillchain properties currently active on target.

    //sc timer    -- skillchain window timer.

    //sc step     -- current weaponskill step information.
    
The following commands are related to the added auto skillchain functionality.

    //sc autows -- enables auto weaponskilling and skillchaining, on by default
    
    //sc skipbursts -- skip the burst phase of a skillchain and reopen a skillchain if available, off by default
    
    //sc setws -- set the weaponskills available for a given step, starts at index 0 for opening a skillchain, 1 for first step, 2 for second step etc
               -- multiple weaponskills can be set per step other than the initial opening weaponskill and will be used in the order added if valid for the weaponskill
               -- example configuration, this will open with savage blade, do step 1 with savage or last stand and do step 2 with last stand if those weaponskills                       would confinue the skillchain
                  //sc setws "Savage Blade" 0
                  //sc setws "Savage Blade" 1
                  //sc setws "Last Stand" 1
                  //sc setws "Last Stand" 2
                  
     //sc printws -- prints the current auto weaponskill configuration
     
     //sc clearws -- clears all currently set ws
     
     //sc saveset setname -- saves the current auto weaponskill configuration to the set name, if the name is default the set will be loaded when the addon loads
     
     //sc saveset setname -- loads the weaponskill set with the given name
     
     //sc deleteset setname -- deletes the set with the given name
     
     //sc printsets -- prints a list of all available set names to chat

More settings related to text object can be found within the settings.xml, generated on addon load
