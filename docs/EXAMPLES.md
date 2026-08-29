# 📝 Examples – AIRIS-AI (All Free)

## Creating a Custom Tool (All Users – Free, No Sponsorship)

```typescript
ipcMain.handle('my-custom-tool', async (event, data) => {
  try {
    const result = await someNativeAction(data);
    return { success: true, data: result };
  } catch (e) {
    return { success: false, error: e.message };
  }
});
```
