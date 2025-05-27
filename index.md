# Testing headings
## Testiong heading type 2
### Really testing the headings
#### Why not a fourth heading
##### Five headings is getting a bit much
###### Six headings is definitely too many

I have started testing the syntax of markdown - it's quite nice actually and I like it especially in GitHub so far.

![Testing image functionality of markdown](https://picsum.photos/id/237/200/300)

~~~python
fig, axs = plt.subplots(2, 2, figsize = (6.4, 4.8))
loss = axs[0, 0].imshow(D1_loss, vmin = -np.max(D1_loss + 100), vmax = np.max(D1_loss + 100),cmap='seismic_r')
axs[0, 0].annotate(r"(a)", xytext = (2200, 250), xy = (2200, 250))
axs[0, 0].set_xticks([0, 750, 1500, 2250])
axs[0, 0].set_xticklabels([0, 750, 1500, 2250])
axs[0, 0].set_yticks([0, 400, 800, 1200])
axs[0, 0].set_yticklabels([0, 400, 800, 1200])
colorbar1 = plt.colorbar(loss, ax = axs[0, 0], shrink = 0.6)
colorbar1.set_ticks([-300, -150, 0, 150, 300])
colorbar1.set_ticklabels([-300, -150, 0, 150, 300])


signal = axs[0, 1].imshow(D1_signal, vmin = -np.max(D1_signal + 100), vmax = np.max(D1_signal + 100),cmap='seismic_r')
axs[0, 1].annotate(r"(b)", xytext = (2200, 250), xy = (2200, 250))
axs[0, 1].set_xticks([0, 750, 1500, 2250])
axs[0, 1].set_xticklabels([0, 750, 1500, 2250])
axs[0, 1].set_yticks([0, 400, 800, 1200])
axs[0, 1].set_yticklabels([0, 400, 800, 1200])
colorbar2 = plt.colorbar(signal, ax = axs[0, 1], shrink = 0.6)
colorbar2.set_ticks([-400, -200, 0, 200, 400])
colorbar2.set_ticklabels([-400, -200, 0, 200, 400])


signal = axs[1, 0].imshow(interleaved_loss, vmin = -np.max(interleaved_loss + 100), vmax = np.max(interleaved_loss + 100),cmap='seismic_r')
axs[1, 0].annotate(r"(c)", xytext = (2200, 250), xy = (2200, 250))
axs[1, 0].set_xticks([0, 750, 1500, 2250])
axs[1, 0].set_xticklabels([0, 750, 1500, 2250])
axs[1, 0].set_yticks([0, 400, 800, 1200])
axs[1, 0].set_yticklabels([0, 400, 800, 1200])
colorbar3 = plt.colorbar(signal, ax = axs[1, 0], shrink = 0.6)
colorbar3.set_ticks([-500, -250, 0, 250, 500])
colorbar3.set_ticklabels([-500, -250, 0, 250, 500])



signal = axs[1, 1].imshow(interleaved_signal, vmin = -np.max(interleaved_signal + 100), vmax = np.max(interleaved_signal + 100),cmap='seismic_r')
axs[1, 1].annotate(r"(d)", xytext = (2200, 250), xy = (2200, 250))
axs[1, 1].set_xticks([0, 750, 1500, 2250])
axs[1, 1].set_xticklabels([0, 750, 1500, 2250])
axs[1, 1].set_yticks([0, 400, 800, 1200])
axs[1, 1].set_yticklabels([0, 400, 800, 1200])
colorbar4 = plt.colorbar(signal, ax = axs[1, 1], shrink = 0.6)
colorbar4.set_ticks([-800, -400, 0, 400, 800])
colorbar4.set_ticklabels([-800, -400, 0, 400, 800])

plt.tight_layout()

plt.savefig("C:\\Users\\xxvh83\\Documents\\Reports\\First Year\\MicroscopeImages\\FinalFigures\\InterleavedCooling\\CombinedPython.png", 
            transparent = None, dpi = 'figure', bbox_inches = 'tight')
plt.show()
~~~
