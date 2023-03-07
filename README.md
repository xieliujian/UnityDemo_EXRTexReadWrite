# UnityDemo_EXRTexReadWrite

## EXR贴图的读写

使用包装的EXRTexture2D类读取exr的贴图

```C#

 // 包装的EXR贴图类
 public class EXRTexture2D
 {
    
        /// <summary>
        /// 贴图宽度
        /// </summary>
        int m_Width;

        /// <summary>
        /// 贴图高度
        /// </summary>
        int m_Height;

        /// <summary>
        /// 数据列表
        /// </summary>
        Color[] m_DataArray;

        /// <summary>
        /// 保存
        /// </summary>
        public unsafe void Save(string path)

        /// <summary>
        /// 加载
        /// </summary>
        /// <param name="path"></param>
        public unsafe void Load(string path)

         /// <summary>
        /// 获取像素
        /// </summary>
        /// <param name="x"></param>
        /// <param name="y"></param>
        /// <returns></returns>
        public Color GetPixel(int x, int y, bool isYFlip = false)

        /// <summary>
        /// 设置像素
        /// </summary>
        /// <param name="x"></param>
        /// <param name="y"></param>
        public void SetPixel(int x, int y, Color color, bool isYFlip = false)


        /// <summary>
        /// 获取像素范围
        /// </summary>
        /// <param name="sx"></param>
        /// <param name="sy"></param>
        /// <param name="w"></param>
        /// <param name="h"></param>
        /// <returns></returns>
        public Color[] GetPixels(int sx, int sy, int w, int h)

        /// <summary>
        /// 设置像素范围
        /// </summary>
        /// <param name="sx"></param>
        /// <param name="sy"></param>
        /// <param name="w"></param>
        /// <param name="h"></param>
        /// <param name="result"></param>
        public void SetPixels(int sx, int sy, int w, int h, Color[] result)

        ...

 }

```


 