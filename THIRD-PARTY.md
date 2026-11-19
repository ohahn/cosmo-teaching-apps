# Third-party components and data

## d3 (bundled in every app)

d3 v7.9.0, https://d3js.org, Copyright 2010-2023 Mike Bostock, under the ISC licence:

> Permission to use, copy, modify, and/or distribute this software for any purpose with or
> without fee is hereby granted, provided that the above copyright notice and this permission
> notice appear in all copies.
>
> THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS
> SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE
> AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
> WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
> NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE
> OF THIS SOFTWARE.

The ISC licence is compatible with the GPL; the notice is also included in each app file.

## Data and methods

- **CMB app:** binned TT, TE and EE power spectra from the Planck 2018 release (Planck Legacy
  Archive, ESA and the Planck Collaboration). The spectra on the sliders come from a neural-network
  emulator trained on runs of the Boltzmann code CLASS (Lesgourgues 2011; Blas, Lesgourgues &
  Tram 2011).
- **BBN app:** observed primordial abundances from the Particle Data Group review
  "Big-Bang nucleosynthesis" (Fields, Molaro & Sarkar, PDG 2024).
- **N-body app:** the FastPM time-stepping scheme (Feng et al. 2016), the Eisenstein & Hu (1998)
  transfer function and halofit (Takahashi et al. 2012), implemented from the published papers.
