These are my combined mods for the II/+ head version (the 5150II and 6505+ are exactly the same except for the name). The lead channel is the same as the earlier 5150/6505 head except for three capacitors and a resistor. The rhythm channel is completely different, using a separate 12AX7 rather than swapping out circuit values inside the lead channel gain structure.

The 6505+ 112 combo is a completely different amp, and these mods are only vaguely applicable to it. The Fender-made 5150 III models are also completely different amps, so don’t try these changes on them either.

Disclaimer: DO THESE MODIFICATIONS AT YOUR OWN RISK. YOU SHOULD KNOW HOW TO WORK SAFELY ON HIGH-VOLTAGE CIRCUITS BEFORE ATTEMPTING THESE. I will NOT provide free support for DIYers doing these mods or adapting them for other amps, so please do not ask (no attitude here, I just can’t afford to do uncompensated labor). I developed all of these mods myself via circuit modeling and experimentation (they are not a knockoff of Voodoo or FJA, which I have never heard nor seen in person), and I’m posting them for informational purposes. If you need help, I can do these mods for you at an affordable price. Finally, on a personal note: respect your local tradesperson. Please don’t hand your tech a printout of this post and ask him/her to do everything, and then get mad when she/he quotes you $500. When I do this work for clients, I target the interventions according to their needs and specific use cases, to maximize their investment return based on my experience.

Oh, and one other thing – if you do these mods and like the results, please give credit where it’s due and link to this post from any videos/blog posts/social media posts you do about your amp. I shouldn’t have to say this, but apparently I do: please don’t pass this material off as your own work!

## Supply & power stage

*   Add a choke. I use a 10H/200mA (Hammond 193J, though it’s obnoxiously large – Mercury makes a smaller one). Replace R210 with the choke.
*   Move the standby switch. Short position S1, cut one of the PT B+ secondary legs and insert the standby there (wire that connects to F1).
*   Replace screen resistors with 1K/5W.
*   Change R68 to 5.6K to get a better bias range.

## Input stage

*   Short R27 and C15. The Soldano SLO100 and high-gain Marshalls just use a 68k grid stop and don’t worry about the rest.
*   Increase R2 to 220K

## Lead channel

*   In the 5150, C17 is a 2n2 cap and 470K resistor in parallel. In the 5150II, it’s a 470pf cap. The former is the SLO100 value, and gives you more bass and thicker voicing (think metalcore). The latter gives you a tight ‘klank’ sound on palm mutes and more nasal snarl (think death metal or 'djent’). I have both options mounted to a switch. The switch has a 8.2M resistor across it to eliminate popping.
*   Increase C2 to .022uF, which is the 5150/SLO100 value. The loss of bass from using .001uF here is frustrating. Just the 470pf cap’s highpass in the previous stage is plenty 'tight’ for death metal etc.
*   Change R4 to a carbon comp for sweetness. No noise penalty because the signal is knocked down 10:1 immediately after the stage.
*   Change R93 to 2K. Biases the EQ driver a little hotter.
*   Change R94 to 47K or 68K (I like 68K). Increases mid presence and thickness, moves lead tone toward SLO 'vocal’ quality with a lot less scoop and boom.
*   Add 500pf-1.5nF cap in parallel with R94. Cuts fizz. I like 1nF here, because in combination with 68K at R94, it keeps a lot of the 'snarl’ treble but dumps most of the fizz without making the sound dull. Makes the amp feel clearer and less mushy on the lead attack, though this is an illusion in some ways.
*   C14 is 470pf in the 5150II and SLO. The earlier 5150 adds a 100pf cap in parallel with it for 570pf total. I like it at 470pf.

## Clean channel

*   C27 is a mid/treble bleed cap on the gain pot. It’s responsible for the horrible boxy sound of this channel at lower gain settings. Cut it out, or replace it with a 100pf-1nf cap for brightness. I like 390pf with the other selections I’ve made below.
*   Replace R154 with 1M if you use 1nf or less for C27. This will restore most of the gain you lose from cutting C27.
*    If the above mods cause the clean sound to be too clean and quiet relative to the crunch sound, change: R23 to 10K, C63 to .047uF, and R174 to 33K. This will give you about 4dB more gain in clean mode without affecting the crunch mode. I found this made switching between the two feel much more natural after the above mods, but left the tone alone.
*    If you want more deep bass in the clean (but not crunch), cut out R174 entirely. This gets the clean into Fenderish territory with real 'V-shape’ prior to the gainstage. I like this with my other selections above and below.
*    To move the mid dip a little higher in frequency, you can lower the value of C63. This change will make it seem like there’s a little more low-mid content in the clean sound, and shave off some of the 'quack’ at lower gain settings where higher values of C27 dominate the sound. My amp has 33nf here, but you could go as low as 22nf.
*    For tighter crunch (but not clean) sound, lower C13 to 1nf. This is not as huge a change as you might think, but makes the crunch more Marshall-y. Only do this if you’ve removed or drastically lowered C27. I prefer the stock 2.2nF value here. Alternatively, you could do a 1nf in parallel with a 470k-1nf series pair, to create a shelving filter and split the difference.
*    Replace R150 and R170 with carbon comps if desired. No noise penalty because lots of signal is thrown away immediately before the EQ. Of the two, you’ll get more mileage out of changing R170.
*    Change R158 and R155 to 2K. Biases both triodes slightly hotter.
*    Increase C166 to 10uF for full-range bass if that’s important to you. This will only be audible with baritone instruments. I left mine at the stock 2.2uF.
*    'Bright’ mode is actually the normal tone stack sound; when you turn it off, treble is being dumped before the EQ. I found that changing R75 to 47k (you could even do 100k here) and R159 to 10M made the non-bright sound much less muffled, but still different from bright, and useful in its own right.
*    To cut some fizz from the crunch (but not clean) sound, add a 1-3.3nf cap in parallel with R157. I like 1nf, which is pretty subtle, but you can definitely go higher to cut more fizz.
*    Remove C150 to get tone stack to standard Marshall values. I left mine alone because I like the more midrange-centric tone the higher value gives, which makes it match better with the lead channel.
*    If the clean is still too quiet relative to the crunch, you can lower the value of R163 from the stock 33k to 22k or even 15k. Mine is 27k.
*    If you find the crunch sounds too dark and “woolly” when you have the clean set properly, you can cut out R157 (stock 82k) to make the crunch a little brighter and more mid-centric relative to the clean. It will also make the crunch a hair louder.

## FX loop & phase inverter

*    Remove C158. This is a treble boost at 10k on the FX recovery stage. Not needed and contributes to fizziness. If you do nothing else on this list, do this!
*    R46 and R58 were carbon film in my amp. I replaced them with metal film for temperature stability and because I’m anal.
*    Add a 47pf cap between pins 1 and 6 of V4. This is in the SLO and most Marshalls. Gets rid of some hiss and makes the output stage a little more stable.
*    You can short R48 if you want, to get the SLO value. The SLO does not have a grid stop on the phase inverter input (and neither do most Marshalls). Or lower it to 10K, which is a more standard value. I left it alone. It may help reduce bad-sounding distortion when the phase inverter is overdriven, and because the phase inverter is boot-strapped, its input impedance is high enough that 100k will not cause undue treble roll-off.

[Link to schematic]

## A word about the presence/resonance circuits

Presence and resonance are frequency-selective controls that, when turned up, reduce negative feedback around the power stage. When NFB is reduced at one frequency relative to another, gain increases at that frequency, along with output impedance (meaning less control over the speakers’ motion). Both controls at zero produces roughly flat frequency response and maximum 'tightness’. Turning them both up produces a 'V’ EQ curve in the power stage with less ability to dampen the speaker’s motion.

The ranges of the two controls are nearly continuous, that is, the presence control rolls in not too far above where the resonance rolls out. I didn’t like this because it seemed to swamp the tone stack settings; the resonance was boomy and the presence was quacky. I opted to move the ranges further apart.

You can lower the corner frequency of the resonance controls by increasing C12 (clean) and C60 (lead). Try 8.2nF or 10nF. I used 10nF since that moved the corner nearly an octave lower. The resonance is now useful for compensating for cabinet rolloff – making a 2x12 sound more like a 4x12.

The presence range is determined by parallel combinations of C8/C62 (clean) and C161/C162 (lead). These combos are .1uF+.033uF, yielding .133uF total. I like just .1uF, but you can alter it in either direction. .1uF or maybe 82nF seems to be more useful for compensating for dark speakers to get more articulation and cut, without bumping the mids as much. Given that I had already modded the amp to have more vocal mids and less treble, .1uF works better than stock.

Many people also notice that the resonance control’s range is smooth, while the presence control seems to 'wake up’ only in the last 3rd of its rotation. This is because both pots are audio taper, but are working in opposite directions – resonance is a series resistance, presence is a shunt to ground. The presence pot should be linear or reverse-audio. I replaced my presence pots with 10K reverse-audio, and their range became much more useful.

## A word about the FX loop

There is a huge amount of misinformation out there about the FX loop. It is NOT parallel, it is a SERIES LOOP. Yes there is some crosstalk around it when the amp is at bedroom level, but it is negligible at recording/stage volume. Remember that the master volume comes before the loop, so the loop is always at “max” into the power stage. There’s a little bit of capacitive coupling around the MV, which is amplified by the loop’s return, even if your outboard gear is muted. It will never get louder than a whisper; it’s not worth worrying about.

The loop is NOT passive like many internet forumites claim; it IS tube-buffered. V3B is an AC-coupled cathode follower, which provides a buffered, low-impedance output for the send. V3A is a recovery stage with a gain of ~15. The confusion arises because V3B/V3A are ALWAYS ON and IN CIRCUIT, what is being switched is the jacks. If you have a footswitch, it is controlling a relay that simply hard-bypasses the output of V3B’s CF straight to the input of V3A’s gain stage. If you don’t, the signal is always routed to the FX jacks, through their switching contacts, again, straight from V3B to V3A.

Both channels knock the signal level down about 10:1 before their EQ networks, so the CF buffer is never overdriven. The buffered output is guitar level (-10dBV nominal) for pedals, NOT line level for rack gear. Because the loop level is so low, it is highly susceptible to noise. Use the shortest/best cables you can, and do NOT sit your effects on top of the amp where they can pick up hum from the power transformer. The other thing is that the grounds of your patch cables form a ground loop from send to return, which picks up hum and buzz. Keep the send and return cables as physically close to each other as possible, to minimize the area of the loop. You can also use a special cable for the send with the ground disconnected at one end.

The CF buffer output has a 2nd-order (2-pole) highpass filter with a corner frequency of about 10Hz. For some reason, certain New Sensor-made tubes appear to have trouble with this, and lose bass response when external effects are patched into the loop (although they’re fine with external effects disconnected). If the external load is heavy (<100K), the corner frequency of the filter shifts, which may or may not be audible.

The recovery stage gets the signal level from guitar level back up to line level to drive the phase inverter. This triode is not intended to be overdriven, and does not sound good when it is. The preamp-out jack on the back of the amp is actually taken AFTER the recovery stage, so it is nominally line level. However, it has a high output impedance (on the order of 150K) so you need a DI box/buffer if it’s going into a low-Z input.

12AU7 conversion:
Dropping a 12AU7 in V3 for the loop won’t hurt anything (and MAY help with driving low-Z effects), but it WILL change the sound of the amp because the 12AU7 biases differently, and affects supply voltages throughout the preamp. 12AU7s draw about 3-5x the current of a 12AX7 at the same circuit values, so you lose about 74V from the B+ when you plug one in. If you actually need to drive inputs that require this kind of current, then you can use 47K/1W load resistors and 2.2K (or 2.7k if you want perfect center-biasing for maximum signal swing) cathode resistors for both the send and return stages, and fully bypass the return cathode by changing C159 to a 22uF. If you’re driving loads as low as 10k, use a 1.5k for R80. This will get you a lower output impedance for both stages in the loop (better noise rejection), lots more current capacity on the send, more headroom, more transparency, and precisely the same recovery gain as the original 12AX7 setup. I left C159 out in my amp with a 12AU7 (about -5dB relative to stock 12AX7 with 2.7k in R14), because I didn’t need all of the recovery gain. To keep the rest of the amp sounding the same, replace R60 with a 10K/5W to get supply voltages back up to where they were before. Raise C53 and C65 to 1uF/400V film caps to keep the low end intact for really heavy loads. Note that the sound of the amp will change slightly regardless, because the 12AU7 will produce more 2nd harmonic than a 12AX7 in this role, but far less 3rd and higher harmonics. I have not found this to be a bad thing.

## A word about tubes

Beyond not using a New Sensor 12AX7 in V3 (FX loop), I tried lots of different tubes in the amp.

For power tubes, JJ 6L6GCs performed the best in terms of power. They put out 110W before clipping. Ruby 6L6s did 95W before clipping, Sovtek 5881s did 90W, and EH/Sovtek 6L6s did 100W. I found the tone to be indistinguishable among power tube types at any reasonable volume, though I had already controlled for the fact that they bias slightly differently.

For preamp tubes, I like the JJ ECC83S best across the board. I tried the JJ 803S in the clean channel and in V1, and was not impressed. It was nasal and spitty-sounding by comparison. EH/Sovteks sounded fizzy and were noisier than the short-plate JJs. Tung-Sols (made by Sovtek) had a nice bite to them, and sounded great in V2 and V5, but had very squishy bass response at any position. Several of them hummed in the amp.

## Voltages

For reference, these are the voltages in my amp (with the 12AU7 conversion):
B+ node 445V (both plate and screen, via choke)
V3+ node 388V
V2+ node 314V
V1+ node 287V