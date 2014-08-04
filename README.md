# solarized-pack

An [Emacs Live](http://overtone.github.io/emacs-live/) pack containing the Solarized color themes.

The Solarized theme is taken (as `git submodule`) from [bbatsov's Emacs version](https://github.com/bbatsov/solarized-emacs), which is inherited from [Ethan Schoonover's "Solarized" themes](http://ethanschoonover.com/solarized).

## Installing and loading the pack

For cloned Emacs Live configuration (similar for other configurations), follow the steps:

1. `git clone git@github.com:neolee/solarized-pack.git ~/.live-packs/solarized-pack`.
2. `cd ~/.live-packs/solarized-pack && git submodule init && git submodule update`.
3. Open `~/.live-packs/solarized-pack/config/solarized-conf.el` and choose 1 theme from all 2 variants, keep it uncommented.
4. Open `~/.emacs-live.el`, add `~/.live-packs/solarized-pack` into `live-add-packs` list.
5. **IMPORTANT**: remove `stable/colour-pack` from `live-use-packs` list. If you haven't add that, make sure the following snippet is in your `~/.emacs-live.el` file:

  ```
(live-use-packs '(stable/foundation-pack
                  ; stable/colour-pack
                  stable/lang-pack
                  stable/power-pack
                  stable/org-pack
                  stable/git-pack
                  stable/clojure-pack
                  stable/bindings-pack))
  ```

6. Start Emacs and enjoy!