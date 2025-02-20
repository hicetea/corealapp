using System;
using System.Runtime.InteropServices;
using System.Text;

namespace ns11
{
	// Token: 0x0200001F RID: 31
	internal sealed class Class8
	{
		// Token: 0x060000EC RID: 236 RVA: 0x00013B28 File Offset: 0x00011D28
		private static string smethod_0(string string_1)
		{
			StringBuilder stringBuilder = new StringBuilder();
			bool flag = true;
			for (int i = 0; i < string_1.Length; i++)
			{
				int value = Convert.ToInt32(string_1[i]);
				if (!flag)
				{
					stringBuilder.Append(' ');
				}
				stringBuilder.Append(value);
				flag = false;
			}
			return stringBuilder.ToString();
		}

		// Token: 0x060000ED RID: 237 RVA: 0x00013B7C File Offset: 0x00011D7C
		private static string smethod_1(string string_1)
		{
			StringBuilder stringBuilder = new StringBuilder();
			string[] array = string_1.Split(new char[]
			{
				' '
			});
			for (int i = 0; i < array.Length; i++)
			{
				char value = Convert.ToChar(Convert.ToInt32(array[i]));
				stringBuilder.Append(value);
			}
			return stringBuilder.ToString();
		}

		// Token: 0x060000EE RID: 238
		[DllImport("libcns.dll", EntryPoint = "#38")]
		internal static extern Class8.Struct2 libcns_38();

		// Token: 0x060000EF RID: 239
		[DllImport("libcns.dll", EntryPoint = "#8")]
		internal static extern void libcns_8(Class8.Struct2 struct2_0);

		// Token: 0x060000F0 RID: 240
		[DllImport("libcns.dll", EntryPoint = "#40")]
		internal static extern void libcns_40(Class8.Struct2 struct2_0, double double_0);

		// Token: 0x060000F1 RID: 241
		[DllImport("libcns.dll", EntryPoint = "#129")]
		internal static extern void libcns_129(Class8.Struct2 struct2_0, Class8.Enum5 enum5_0);

		// Token: 0x060000F2 RID: 242
		[DllImport("libcns.dll", EntryPoint = "#86")]
		internal static extern void libcns_86(Class8.Struct2 struct2_0, Class8.Enum3 enum3_0);

		// Token: 0x060000F3 RID: 243
		[DllImport("libcns.dll", EntryPoint = "#79")]
		internal static extern void libcns_79(Class8.Struct2 struct2_0, Class8.Enum2 enum2_0);

		// Token: 0x060000F4 RID: 244
		[DllImport("libcns.dll", EntryPoint = "#143")]
		internal static extern void libcns_143(Class8.Struct2 struct2_0, double double_0, double double_1, double double_2);

		// Token: 0x060000F5 RID: 245
		[DllImport("libcns.dll", EntryPoint = "#289")]
		internal static extern void libcns_289(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x060000F6 RID: 246
		[DllImport("libcns.dll", EntryPoint = "#375")]
		internal static extern void libcns_375(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x060000F7 RID: 247
		[DllImport("libcns.dll", EntryPoint = "#10")]
		private static extern void libcns_10(Class8.Struct2 struct2_0, StringBuilder stringBuilder_0);

		// Token: 0x060000F8 RID: 248 RVA: 0x00002B31 File Offset: 0x00000D31
		internal static void smethod_2(Class8.Struct2 struct2_0, string string_1)
		{
			Class8.libcns_10(struct2_0, new StringBuilder(string_1));
		}

		// Token: 0x060000F9 RID: 249
		[DllImport("libcns.dll", EntryPoint = "#14")]
		private static extern void libcns_14(Class8.Struct2 struct2_0, StringBuilder stringBuilder_0);

		// Token: 0x060000FA RID: 250 RVA: 0x00002B3F File Offset: 0x00000D3F
		internal static void smethod_3(Class8.Struct2 struct2_0, string string_1)
		{
			Class8.libcns_14(struct2_0, new StringBuilder(string_1));
		}

		// Token: 0x060000FB RID: 251
		[DllImport("libcns.dll", EntryPoint = "#6")]
		internal static extern Class8.Struct4 libcns_6(Class8.Struct2 struct2_0, int int_0, double double_0, double double_1);

		// Token: 0x060000FC RID: 252
		[DllImport("libcns.dll", EntryPoint = "#116")]
		private static extern Class8.Struct4 libcns_116(Class8.Struct2 struct2_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x060000FD RID: 253 RVA: 0x00002B4D File Offset: 0x00000D4D
		internal static Class8.Struct4 smethod_4(Class8.Struct2 struct2_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			return Class8.libcns_116(struct2_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x060000FE RID: 254
		[DllImport("libcns.dll", EntryPoint = "#118")]
		private static extern void libcns_118(Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x060000FF RID: 255 RVA: 0x00002B5A File Offset: 0x00000D5A
		internal static void smethod_5(Class8.Struct4 struct4_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_118(struct4_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000100 RID: 256
		[DllImport("libcns.dll", EntryPoint = "#363")]
		private static extern void libcns_363(Class8.Struct4 struct4_0, Class8.Struct0 struct0_0, int int_0, [In] Class8.Struct1[] struct1_0, double double_0);

		// Token: 0x06000101 RID: 257 RVA: 0x00002B66 File Offset: 0x00000D66
		internal static void smethod_6(Class8.Struct4 struct4_0, Class8.Struct0 struct0_0, [In] Class8.Struct1[] struct1_0, double double_0)
		{
			Class8.libcns_363(struct4_0, struct0_0, struct1_0.Length, struct1_0, double_0);
		}

		// Token: 0x06000102 RID: 258
		[DllImport("libcns.dll", EntryPoint = "#70")]
		private static extern Class8.Struct4 libcns_70(Class8.Struct2 struct2_0, int int_0, int int_1, [In] Class8.Struct0[] struct0_0);

		// Token: 0x06000103 RID: 259 RVA: 0x00002B74 File Offset: 0x00000D74
		internal static Class8.Struct4 smethod_7(Class8.Struct2 struct2_0, int int_0, [In] Class8.Struct0[] struct0_0)
		{
			return Class8.libcns_70(struct2_0, int_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x06000104 RID: 260
		[DllImport("libcns.dll", EntryPoint = "#72")]
		private static extern void libcns_72(Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct0[] struct0_0);

		// Token: 0x06000105 RID: 261 RVA: 0x00002B81 File Offset: 0x00000D81
		internal static void smethod_8(Class8.Struct4 struct4_0, [In] Class8.Struct0[] struct0_0)
		{
			Class8.libcns_72(struct4_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x06000106 RID: 262
		[DllImport("libcns.dll", EntryPoint = "#102")]
		private static extern void libcns_102(Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct0[] struct0_0);

		// Token: 0x06000107 RID: 263 RVA: 0x00002B8D File Offset: 0x00000D8D
		internal static void smethod_9(Class8.Struct4 struct4_0, [In] Class8.Struct0[] struct0_0)
		{
			Class8.libcns_102(struct4_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x06000108 RID: 264
		[DllImport("libcns.dll", EntryPoint = "#120")]
		private static extern void libcns_120(Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000109 RID: 265 RVA: 0x00002B99 File Offset: 0x00000D99
		internal static void smethod_10(Class8.Struct4 struct4_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_120(struct4_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x0600010A RID: 266
		[DllImport("libcns.dll", EntryPoint = "#46")]
		internal static extern void libcns_46(Class8.Struct4 struct4_0, double double_0, double double_1, double double_2, double double_3);

		// Token: 0x0600010B RID: 267
		[DllImport("libcns.dll", EntryPoint = "#367")]
		internal static extern void libcns_367(Class8.Struct4 struct4_0, double double_0, double double_1, double double_2, double double_3, double double_4);

		// Token: 0x0600010C RID: 268
		[DllImport("libcns.dll", EntryPoint = "#68")]
		internal static extern void libcns_68(Class8.Struct4 struct4_0, int int_0);

		// Token: 0x0600010D RID: 269
		[DllImport("libcns.dll", EntryPoint = "#98")]
		internal static extern void libcns_98(Class8.Struct4 struct4_0, Class8.Enum4 enum4_0);

		// Token: 0x0600010E RID: 270
		[DllImport("libcns.dll", EntryPoint = "#58")]
		private static extern void libcns_58(Class8.Struct4 struct4_0, StringBuilder stringBuilder_0);

		// Token: 0x0600010F RID: 271 RVA: 0x00002BA5 File Offset: 0x00000DA5
		internal static void smethod_11(Class8.Struct4 struct4_0, string string_1)
		{
			Class8.libcns_58(struct4_0, new StringBuilder(Class8.smethod_0(string_1)));
		}

		// Token: 0x06000110 RID: 272
		[DllImport("libcns.dll", EntryPoint = "#110")]
		private static extern Class8.Struct3 libcns_110(Class8.Struct2 struct2_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000111 RID: 273 RVA: 0x00002BB8 File Offset: 0x00000DB8
		internal static Class8.Struct3 smethod_12(Class8.Struct2 struct2_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			return Class8.libcns_110(struct2_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000112 RID: 274
		[DllImport("libcns.dll", EntryPoint = "#42")]
		internal static extern void libcns_42(Class8.Struct3 struct3_0, bool bool_0, bool bool_1, double double_0);

		// Token: 0x06000113 RID: 275
		[DllImport("libcns.dll", EntryPoint = "#127")]
		internal static extern void libcns_127(Class8.Struct3 struct3_0, int int_0);

		// Token: 0x06000114 RID: 276
		[DllImport("libcns.dll", EntryPoint = "#112")]
		private static extern void libcns_112(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000115 RID: 277 RVA: 0x00002BC5 File Offset: 0x00000DC5
		internal static void smethod_13(Class8.Struct3 struct3_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_112(struct3_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000116 RID: 278
		[DllImport("libcns.dll", EntryPoint = "#114")]
		private static extern void libcns_114(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000117 RID: 279 RVA: 0x00002BD1 File Offset: 0x00000DD1
		internal static void smethod_14(Class8.Struct3 struct3_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_114(struct3_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000118 RID: 280
		[DllImport("libcns.dll", EntryPoint = "#125")]
		private static extern void libcns_125(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, int int_0, [In] Class8.Struct1[] struct1_0, double double_0);

		// Token: 0x06000119 RID: 281 RVA: 0x00002BDD File Offset: 0x00000DDD
		internal static void smethod_15(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, [In] Class8.Struct1[] struct1_0, double double_0)
		{
			Class8.libcns_125(struct3_0, struct0_0, struct1_0.Length, struct1_0, double_0);
		}

		// Token: 0x0600011A RID: 282
		[DllImport("libcns.dll", EntryPoint = "#4")]
		private static extern Class8.Struct3 libcns_4(Class8.Struct2 struct2_0, int int_0, int int_1, [In] Class8.Struct0[] struct0_0);

		// Token: 0x0600011B RID: 283 RVA: 0x00002BEB File Offset: 0x00000DEB
		internal static Class8.Struct3 smethod_16(Class8.Struct2 struct2_0, int int_0, [In] Class8.Struct0[] struct0_0)
		{
			return Class8.libcns_4(struct2_0, int_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x0600011C RID: 284
		[DllImport("libcns.dll", EntryPoint = "#2")]
		private static extern void libcns_2(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct0[] struct0_0);

		// Token: 0x0600011D RID: 285 RVA: 0x00002BF8 File Offset: 0x00000DF8
		internal static void smethod_17(Class8.Struct3 struct3_0, [In] Class8.Struct0[] struct0_0)
		{
			Class8.libcns_2(struct3_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x0600011E RID: 286
		[DllImport("libcns.dll", EntryPoint = "#104")]
		private static extern void libcns_104(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct0[] struct0_0);

		// Token: 0x0600011F RID: 287 RVA: 0x00002C04 File Offset: 0x00000E04
		internal static void smethod_18(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct0[] struct0_0)
		{
			Class8.libcns_104(struct3_0, struct0_0.Length, struct0_0);
		}

		// Token: 0x06000120 RID: 288
		[DllImport("libcns.dll", EntryPoint = "#135")]
		internal static extern Class8.Struct3 libcns_135(Class8.Struct2 struct2_0, int int_0, double double_0, double double_1, double double_2, double double_3);

		// Token: 0x06000121 RID: 289
		[DllImport("libcns.dll", EntryPoint = "#131")]
		internal static extern Class8.Struct3 libcns_131(Class8.Struct2 struct2_0, int int_0, double double_0, double double_1, double double_2);

		// Token: 0x06000122 RID: 290
		[DllImport("libcns.dll", EntryPoint = "#133")]
		internal static extern void libcns_133(Class8.Struct3 struct3_0, double double_0, double double_1, double double_2);

		// Token: 0x06000123 RID: 291
		[DllImport("libcns.dll", EntryPoint = "#137")]
		internal static extern void libcns_137(Class8.Struct3 struct3_0, double double_0, double double_1, double double_2, double double_3);

		// Token: 0x06000124 RID: 292
		[DllImport("libcns.dll", EntryPoint = "#261")]
		internal static extern void libcns_261(Class8.Struct3 struct3_0, double double_0, double double_1, double double_2);

		// Token: 0x06000125 RID: 293
		[DllImport("libcns.dll", EntryPoint = "#263")]
		internal static extern void libcns_263(Class8.Struct3 struct3_0, double double_0, double double_1, double double_2, double double_3);

		// Token: 0x06000126 RID: 294
		[DllImport("libcns.dll", EntryPoint = "#138")]
		internal static extern void libcns_138(Class8.Struct3 struct3_0, int int_0);

		// Token: 0x06000127 RID: 295
		[DllImport("libcns.dll", EntryPoint = "#145")]
		internal static extern void libcns_145(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000128 RID: 296
		[DllImport("libcns.dll", EntryPoint = "#94")]
		internal static extern void libcns_94(Class8.Struct3 struct3_0, bool bool_0, double double_0, double double_1);

		// Token: 0x06000129 RID: 297
		[DllImport("libcns.dll", EntryPoint = "#44")]
		private static extern void libcns_44(Class8.Struct3 struct3_0, StringBuilder stringBuilder_0);

		// Token: 0x0600012A RID: 298 RVA: 0x00002C10 File Offset: 0x00000E10
		internal static void smethod_19(Class8.Struct3 struct3_0, string string_1)
		{
			Class8.libcns_44(struct3_0, new StringBuilder(Class8.smethod_0(string_1)));
		}

		// Token: 0x0600012B RID: 299
		[DllImport("libcns.dll", EntryPoint = "#36")]
		private static extern Class8.Struct7 libcns_36(Class8.Struct2 struct2_0, StringBuilder stringBuilder_0, StringBuilder stringBuilder_1, double double_0);

		// Token: 0x0600012C RID: 300 RVA: 0x00002C23 File Offset: 0x00000E23
		internal static Class8.Struct7 smethod_20(Class8.Struct2 struct2_0, string string_1, string string_2, double double_0)
		{
			return Class8.libcns_36(struct2_0, new StringBuilder(string_1), new StringBuilder(string_2), double_0);
		}

		// Token: 0x0600012D RID: 301
		[DllImport("libcns.dll", EntryPoint = "#52")]
		internal static extern Class8.Struct7 libcns_52(Class8.Struct2 struct2_0, double double_0);

		// Token: 0x0600012E RID: 302
		[DllImport("libcns.dll", EntryPoint = "#48")]
		internal static extern Class8.Enum1 libcns_48(Class8.Struct7 struct7_0);

		// Token: 0x0600012F RID: 303
		[DllImport("libcns.dll", EntryPoint = "#50")]
		internal static extern Class8.Enum1 libcns_50(Class8.Struct7 struct7_0);

		// Token: 0x06000130 RID: 304
		[DllImport("libcns.dll", EntryPoint = "#16")]
		internal static extern Class8.Enum1 libcns_16(Class8.Struct7 struct7_0);

		// Token: 0x06000131 RID: 305
		[DllImport("libcns.dll", EntryPoint = "#123")]
		internal static extern Class8.Enum1 libcns_123(Class8.Struct7 struct7_0);

		// Token: 0x06000132 RID: 306
		[DllImport("libcns.dll", EntryPoint = "#54")]
		internal static extern Class8.Enum1 libcns_54(Class8.Struct7 struct7_0);

		// Token: 0x06000133 RID: 307
		[DllImport("libcns.dll", EntryPoint = "#253")]
		internal static extern void libcns_253(Class8.Struct2 struct2_0);

		// Token: 0x06000134 RID: 308
		[DllImport("libcns.dll", EntryPoint = "#34")]
		internal static extern Class8.Struct5 libcns_34(Class8.Struct7 struct7_0);

		// Token: 0x06000135 RID: 309
		[DllImport("libcns.dll", EntryPoint = "#12")]
		private static extern void libcns_12(Class8.Struct5 struct5_0, StringBuilder stringBuilder_0);

		// Token: 0x06000136 RID: 310 RVA: 0x00002C38 File Offset: 0x00000E38
		internal static void smethod_21(Class8.Struct5 struct5_0, string string_1)
		{
			Class8.libcns_12(struct5_0, new StringBuilder(string_1));
		}

		// Token: 0x06000137 RID: 311
		[DllImport("libcns.dll", EntryPoint = "#225")]
		private static extern void libcns_225(Class8.Struct6 struct6_0, StringBuilder stringBuilder_0);

		// Token: 0x06000138 RID: 312 RVA: 0x00002C46 File Offset: 0x00000E46
		internal static void smethod_22(Class8.Struct6 struct6_0, string string_1)
		{
			Class8.libcns_225(struct6_0, new StringBuilder(string_1));
		}

		// Token: 0x06000139 RID: 313
		[DllImport("libcns.dll", EntryPoint = "#26")]
		internal static extern int libcns_26(Class8.Struct5 struct5_0);

		// Token: 0x0600013A RID: 314
		[DllImport("libcns.dll", EntryPoint = "#22")]
		internal static extern Class8.Struct6 libcns_22(Class8.Struct5 struct5_0, int int_0);

		// Token: 0x0600013B RID: 315
		[DllImport("libcns.dll", EntryPoint = "#18")]
		internal static extern int libcns_18(Class8.Struct6 struct6_0);

		// Token: 0x0600013C RID: 316
		[DllImport("libcns.dll", EntryPoint = "#32")]
		internal static extern Class8.Struct4 libcns_32(Class8.Struct6 struct6_0);

		// Token: 0x0600013D RID: 317
		[DllImport("libcns.dll", EntryPoint = "#24")]
		internal static extern int libcns_24(Class8.Struct6 struct6_0);

		// Token: 0x0600013E RID: 318
		[DllImport("libcns.dll", EntryPoint = "#20")]
		internal static extern void libcns_20(Class8.Struct6 struct6_0, int int_0, ref Class8.Struct3 struct3_0, ref double double_0, ref double double_1, ref bool bool_0, ref double double_2);

		// Token: 0x0600013F RID: 319
		[DllImport("libcns.dll", EntryPoint = "#60")]
		private static extern IntPtr libcns_60(Class8.Struct4 struct4_0);

		// Token: 0x06000140 RID: 320 RVA: 0x00002C54 File Offset: 0x00000E54
		internal static string smethod_23(Class8.Struct4 struct4_0)
		{
			return Class8.smethod_1(Marshal.PtrToStringAnsi(Class8.libcns_60(struct4_0)));
		}

		// Token: 0x06000141 RID: 321
		[DllImport("libcns.dll", EntryPoint = "#28")]
		private static extern IntPtr libcns_28(Class8.Struct3 struct3_0);

		// Token: 0x06000142 RID: 322 RVA: 0x00002C66 File Offset: 0x00000E66
		internal static string smethod_24(Class8.Struct3 struct3_0)
		{
			return Class8.smethod_1(Marshal.PtrToStringAnsi(Class8.libcns_28(struct3_0)));
		}

		// Token: 0x06000143 RID: 323
		[DllImport("libcns.dll", EntryPoint = "#77")]
		internal static extern void libcns_77(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000144 RID: 324
		[DllImport("libcns.dll", EntryPoint = "#163")]
		private static extern void libcns_163(Class8.Struct2 struct2_0, StringBuilder stringBuilder_0, StringBuilder stringBuilder_1);

		// Token: 0x06000145 RID: 325 RVA: 0x00002C78 File Offset: 0x00000E78
		internal static void smethod_25(Class8.Struct2 struct2_0, string string_1, string string_2)
		{
			Class8.libcns_163(struct2_0, new StringBuilder(string_1), new StringBuilder(string_2));
		}

		// Token: 0x06000146 RID: 326
		[DllImport("libcns.dll", EntryPoint = "#81")]
		internal static extern void libcns_81(Class8.Struct4 struct4_0, double double_0);

		// Token: 0x06000147 RID: 327
		[DllImport("libcns.dll", EntryPoint = "#83")]
		internal static extern void libcns_83(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000148 RID: 328
		[DllImport("libcns.dll", EntryPoint = "#85")]
		internal static extern void libcns_85(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000149 RID: 329
		[DllImport("libcns.dll", EntryPoint = "#271")]
		internal static extern void libcns_271(bool bool_0);

		// Token: 0x0600014A RID: 330
		[DllImport("libcns.dll", EntryPoint = "#149")]
		internal static extern void libcns_149(Class8.Struct2 struct2_0, bool bool_0, double double_0);

		// Token: 0x0600014B RID: 331
		[DllImport("libcns.dll", EntryPoint = "#373")]
		internal static extern void libcns_373(Class8.Struct2 struct2_0, bool bool_0, double double_0);

		// Token: 0x0600014C RID: 332
		[DllImport("libcns.dll", EntryPoint = "#167")]
		internal static extern void libcns_167(Class8.Struct3 struct3_0, bool bool_0);

		// Token: 0x0600014D RID: 333
		[DllImport("libcns.dll", EntryPoint = "#395")]
		internal static extern void libcns_395(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x0600014E RID: 334
		[DllImport("libcns.dll", EntryPoint = "#151")]
		internal static extern void libcns_151(Class8.Struct2 struct2_0, Class8.Enum6 enum6_0);

		// Token: 0x0600014F RID: 335
		[DllImport("libcns.dll", EntryPoint = "#153")]
		internal static extern void libcns_153(Class8.Struct2 struct2_0, double double_0, double double_1, Class8.Enum8 enum8_0, bool bool_0, bool bool_1);

		// Token: 0x06000150 RID: 336
		[DllImport("libcns.dll", EntryPoint = "#425")]
		internal static extern void libcns_425(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000151 RID: 337
		[DllImport("libcns.dll", EntryPoint = "#155")]
		internal static extern void libcns_155(Class8.Struct2 struct2_0, Class8.Enum7 enum7_0);

		// Token: 0x06000152 RID: 338
		[DllImport("libcns.dll", EntryPoint = "#157")]
		internal static extern void libcns_157(Class8.Struct2 struct2_0, double double_0, double double_1);

		// Token: 0x06000153 RID: 339
		[DllImport("libcns.dll", EntryPoint = "#345")]
		internal static extern void libcns_345(Class8.Struct2 struct2_0, double double_0);

		// Token: 0x06000154 RID: 340
		[DllImport("libcns.dll", EntryPoint = "#377")]
		internal static extern void libcns_377(Class8.Struct2 struct2_0, double double_0, double double_1);

		// Token: 0x06000155 RID: 341
		[DllImport("libcns.dll", EntryPoint = "#361")]
		internal static extern void libcns_361(Class8.Struct3 struct3_0, int int_0);

		// Token: 0x06000156 RID: 342
		[DllImport("libcns.dll", EntryPoint = "#159")]
		internal static extern int libcns_159(Class8.Struct6 struct6_0);

		// Token: 0x06000157 RID: 343
		[DllImport("libcns.dll", EntryPoint = "#161")]
		internal static extern void libcns_161(Class8.Struct6 struct6_0, int int_0, ref Class8.Struct8 struct8_0, ref int int_1, ref Class8.Struct8 struct8_1, ref int int_2, ref Class8.Struct8 struct8_2);

		// Token: 0x06000158 RID: 344
		[DllImport("libcns.dll", EntryPoint = "#169")]
		internal static extern double libcns_169(Class8.Struct5 struct5_0);

		// Token: 0x06000159 RID: 345
		[DllImport("libcns.dll", EntryPoint = "#171")]
		internal static extern void libcns_171(Class8.Struct6 struct6_0, ref double double_0, ref double double_1);

		// Token: 0x0600015A RID: 346
		[DllImport("libcns.dll", EntryPoint = "#193")]
		internal static extern double libcns_193(Class8.Struct6 struct6_0);

		// Token: 0x0600015B RID: 347
		[DllImport("libcns.dll", EntryPoint = "#181")]
		internal static extern void libcns_181(Class8.Struct3 struct3_0, double double_0);

		// Token: 0x0600015C RID: 348
		[DllImport("libcns.dll", EntryPoint = "#175")]
		internal static extern void libcns_175(Class8.Struct2 struct2_0, bool bool_0, int int_0, double double_0, double double_1, bool bool_1);

		// Token: 0x0600015D RID: 349
		[DllImport("libcns.dll", EntryPoint = "#177")]
		internal static extern void libcns_177(Class8.Struct2 struct2_0, Class8.Enum9 enum9_0, bool bool_0);

		// Token: 0x0600015E RID: 350
		[DllImport("libcns.dll", EntryPoint = "#179")]
		internal static extern void libcns_179(Class8.Struct2 struct2_0, double double_0, double double_1, bool bool_0, double double_2);

		// Token: 0x0600015F RID: 351
		[DllImport("libcns.dll", EntryPoint = "#185")]
		internal static extern void libcns_185(Class8.Struct6 struct6_0, int int_0, ref int int_1, ref int int_2, ref double double_0);

		// Token: 0x06000160 RID: 352
		[DllImport("libcns.dll", EntryPoint = "#183")]
		internal static extern void libcns_183(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000161 RID: 353
		[DllImport("libcns.dll", EntryPoint = "#189")]
		internal static extern void libcns_189(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000162 RID: 354
		[DllImport("libcns.dll", EntryPoint = "#191")]
		internal static extern void libcns_191(Class8.Struct3 struct3_0, Class8.Enum10 enum10_0);

		// Token: 0x06000163 RID: 355
		[DllImport("libcns.dll", EntryPoint = "#187")]
		internal static extern void libcns_187(Class8.Struct2 struct2_0, double double_0, double double_1, double double_2, double double_3, int int_0, double double_4);

		// Token: 0x06000164 RID: 356
		[DllImport("libcns.dll", EntryPoint = "#213")]
		internal static extern void libcns_213(Class8.Struct2 struct2_0, double double_0);

		// Token: 0x06000165 RID: 357
		[DllImport("libcns.dll", EntryPoint = "#147")]
		internal static extern void libcns_147(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000166 RID: 358
		[DllImport("libcns.dll", EntryPoint = "#411")]
		internal static extern void libcns_411(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000167 RID: 359
		[DllImport("libcns.dll", EntryPoint = "#413")]
		internal static extern void libcns_413(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000168 RID: 360
		[DllImport("libcns.dll", EntryPoint = "#223")]
		internal static extern void libcns_223(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000169 RID: 361
		[DllImport("libcns.dll", EntryPoint = "#173")]
		internal static extern void libcns_173(Class8.Struct4 struct4_0, double double_0);

		// Token: 0x0600016A RID: 362
		[DllImport("libcns.dll", EntryPoint = "#299")]
		internal static extern void libcns_299(Class8.Struct4 struct4_0, Class8.Enum3 enum3_0);

		// Token: 0x0600016B RID: 363
		[DllImport("libcns.dll", EntryPoint = "#301")]
		internal static extern void libcns_301(Class8.Struct4 struct4_0, Class8.Enum2 enum2_0);

		// Token: 0x0600016C RID: 364
		[DllImport("libcns.dll", EntryPoint = "#305")]
		internal static extern void libcns_305(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x0600016D RID: 365
		[DllImport("libcns.dll", EntryPoint = "#307")]
		internal static extern void libcns_307(Class8.Struct4 struct4_0, Class8.Struct3 struct3_0, double double_0, double double_1, bool bool_0, double double_2);

		// Token: 0x0600016E RID: 366
		[DllImport("libcns.dll", EntryPoint = "#313")]
		internal static extern void libcns_313(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x0600016F RID: 367
		[DllImport("libcns.dll", EntryPoint = "#317")]
		internal static extern void libcns_317(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000170 RID: 368
		[DllImport("libcns.dll", EntryPoint = "#140")]
		internal static extern void libcns_140(Class8.Struct2 struct2_0, Class8.Enum11 enum11_0);

		// Token: 0x06000171 RID: 369
		[DllImport("libcns.dll", EntryPoint = "#29")]
		internal static extern Class8.Struct3 libcns_29(Class8.Struct7 struct7_0);

		// Token: 0x06000172 RID: 370
		[DllImport("libcns.dll", EntryPoint = "#92")]
		private static extern IntPtr libcns_92();

		// Token: 0x06000173 RID: 371 RVA: 0x00002C8C File Offset: 0x00000E8C
		internal static string smethod_26()
		{
			return Marshal.PtrToStringAnsi(Class8.libcns_92());
		}

		// Token: 0x06000174 RID: 372
		[DllImport("libcns.dll", EntryPoint = "#409")]
		private static extern IntPtr libcns_409();

		// Token: 0x06000175 RID: 373 RVA: 0x00002C98 File Offset: 0x00000E98
		internal static string smethod_27()
		{
			return Marshal.PtrToStringAnsi(Class8.libcns_409());
		}

		// Token: 0x06000176 RID: 374
		[DllImport("libcns.dll", EntryPoint = "#90")]
		private static extern IntPtr libcns_90();

		// Token: 0x06000177 RID: 375 RVA: 0x00002CA4 File Offset: 0x00000EA4
		internal static string smethod_28()
		{
			return Marshal.PtrToStringAnsi(Class8.libcns_90());
		}

		// Token: 0x06000178 RID: 376
		[DllImport("libcns.dll", EntryPoint = "#88")]
		private static extern IntPtr libcns_88();

		// Token: 0x06000179 RID: 377 RVA: 0x00002CB0 File Offset: 0x00000EB0
		internal static string smethod_29()
		{
			return Marshal.PtrToStringAnsi(Class8.libcns_88());
		}

		// Token: 0x0600017A RID: 378
		[DllImport("libcns.dll", EntryPoint = "#165")]
		internal static extern Class8.Struct7 libcns_165(Class8.Struct2 struct2_0);

		// Token: 0x0600017B RID: 379
		[DllImport("libcns.dll", EntryPoint = "#259")]
		internal static extern void libcns_259(Class8.Struct2 struct2_0, bool bool_0, double double_0, double double_1, bool bool_1, double double_2);

		// Token: 0x0600017C RID: 380
		[DllImport("libcns.dll", EntryPoint = "#291")]
		private static extern void libcns_291(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x0600017D RID: 381 RVA: 0x00002CBC File Offset: 0x00000EBC
		internal static void smethod_30(Class8.Struct3 struct3_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_291(struct3_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x0600017E RID: 382
		[DllImport("libcns.dll", EntryPoint = "#297")]
		private static extern void libcns_297(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x0600017F RID: 383 RVA: 0x00002CC8 File Offset: 0x00000EC8
		internal static void smethod_31(Class8.Struct3 struct3_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_297(struct3_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000180 RID: 384
		[DllImport("libcns.dll", EntryPoint = "#295")]
		internal static extern void libcns_295(Class8.Struct3 struct3_0, double double_0);

		// Token: 0x06000181 RID: 385
		[DllImport("libcns.dll", EntryPoint = "#315")]
		private static extern void libcns_315(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, int int_0, [In] Class8.Struct1[] struct1_0, double double_0);

		// Token: 0x06000182 RID: 386 RVA: 0x00002CD4 File Offset: 0x00000ED4
		internal static void smethod_32(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, [In] Class8.Struct1[] struct1_0, double double_0)
		{
			Class8.libcns_315(struct3_0, struct0_0, struct1_0.Length, struct1_0, double_0);
		}

		// Token: 0x06000183 RID: 387
		[DllImport("libcns.dll", EntryPoint = "#365")]
		internal static extern void libcns_365(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x06000184 RID: 388
		[DllImport("libcns.dll", EntryPoint = "#273")]
		internal static extern void libcns_273(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x06000185 RID: 389
		[DllImport("libcns.dll", EntryPoint = "#275")]
		private static extern void libcns_275(Class8.Struct3 struct3_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000186 RID: 390 RVA: 0x00002CE2 File Offset: 0x00000EE2
		internal static void smethod_33(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_275(struct3_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000187 RID: 391
		[DllImport("libcns.dll", EntryPoint = "#277")]
		private static extern void libcns_277(Class8.Struct4 struct4_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000188 RID: 392 RVA: 0x00002CEF File Offset: 0x00000EEF
		internal static void smethod_34(Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_277(struct4_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000189 RID: 393
		[DllImport("libcns.dll", EntryPoint = "#293")]
		private static extern void libcns_293(Class8.Struct3 struct3_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x0600018A RID: 394 RVA: 0x00002CFC File Offset: 0x00000EFC
		internal static void smethod_35(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_293(struct3_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x0600018B RID: 395
		[DllImport("libcns.dll", EntryPoint = "#195")]
		private static extern Class8.Struct9 libcns_195(Class8.Struct3 struct3_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x0600018C RID: 396 RVA: 0x00002D09 File Offset: 0x00000F09
		internal static Class8.Struct9 smethod_36(Class8.Struct3 struct3_0, [In] Class8.Struct1[] struct1_0)
		{
			return Class8.libcns_195(struct3_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x0600018D RID: 397
		[DllImport("libcns.dll", EntryPoint = "#255")]
		internal static extern Class8.Struct9 libcns_255(Class8.Struct3 struct3_0, bool bool_0, double double_0);

		// Token: 0x0600018E RID: 398
		[DllImport("libcns.dll", EntryPoint = "#203")]
		internal static extern void libcns_203(Class8.Struct9 struct9_0, bool bool_0, bool bool_1, double double_0);

		// Token: 0x0600018F RID: 399
		[DllImport("libcns.dll", EntryPoint = "#197")]
		private static extern void libcns_197(Class8.Struct9 struct9_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000190 RID: 400 RVA: 0x00002D15 File Offset: 0x00000F15
		internal static void smethod_37(Class8.Struct9 struct9_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_197(struct9_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000191 RID: 401
		[DllImport("libcns.dll", EntryPoint = "#199")]
		private static extern void libcns_199(Class8.Struct9 struct9_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x06000192 RID: 402 RVA: 0x00002D21 File Offset: 0x00000F21
		internal static void smethod_38(Class8.Struct9 struct9_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_199(struct9_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x06000193 RID: 403
		[DllImport("libcns.dll", EntryPoint = "#201")]
		private static extern void libcns_201(Class8.Struct9 struct9_0, Class8.Struct0 struct0_0, int int_0, [In] Class8.Struct1[] struct1_0, double double_0);

		// Token: 0x06000194 RID: 404 RVA: 0x00002D2D File Offset: 0x00000F2D
		internal static void smethod_39(Class8.Struct9 struct9_0, Class8.Struct0 struct0_0, [In] Class8.Struct1[] struct1_0, double double_0)
		{
			Class8.libcns_201(struct9_0, struct0_0, struct1_0.Length, struct1_0, double_0);
		}

		// Token: 0x06000195 RID: 405
		[DllImport("libcns.dll", EntryPoint = "#205")]
		internal static extern void libcns_205(Class8.Struct9 struct9_0, bool bool_0, double double_0, double double_1);

		// Token: 0x06000196 RID: 406
		[DllImport("libcns.dll", EntryPoint = "#209")]
		internal static extern void libcns_209(Class8.Struct9 struct9_0, StringBuilder stringBuilder_0);

		// Token: 0x06000197 RID: 407 RVA: 0x00002D3B File Offset: 0x00000F3B
		internal static void smethod_40(Class8.Struct9 struct9_0, string string_1)
		{
			Class8.libcns_209(struct9_0, new StringBuilder(string_1));
		}

		// Token: 0x06000198 RID: 408
		[DllImport("libcns.dll", EntryPoint = "#211")]
		private static extern IntPtr libcns_211(Class8.Struct9 struct9_0);

		// Token: 0x06000199 RID: 409 RVA: 0x00002D49 File Offset: 0x00000F49
		internal static string smethod_41(Class8.Struct9 struct9_0)
		{
			return Marshal.PtrToStringAnsi(Class8.libcns_211(struct9_0));
		}

		// Token: 0x0600019A RID: 410
		[DllImport("libcns.dll", EntryPoint = "#207")]
		internal static extern Class8.Struct9 libcns_207(Class8.Struct6 struct6_0, int int_0);

		// Token: 0x0600019B RID: 411
		[DllImport("libcns.dll", EntryPoint = "#279")]
		internal static extern Class8.Struct10 libcns_279(Class8.Struct2 struct2_0);

		// Token: 0x0600019C RID: 412
		[DllImport("libcns.dll", EntryPoint = "#285")]
		private static extern void libcns_285(Class8.Struct10 struct10_0, Class8.Struct4 struct4_0, int int_0, [In] Class8.Struct1[] struct1_0);

		// Token: 0x0600019D RID: 413 RVA: 0x00002D56 File Offset: 0x00000F56
		internal static void smethod_42(Class8.Struct10 struct10_0, Class8.Struct4 struct4_0, [In] Class8.Struct1[] struct1_0)
		{
			Class8.libcns_285(struct10_0, struct4_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x0600019E RID: 414
		[DllImport("libcns.dll", EntryPoint = "#283")]
		internal static extern void libcns_283(Class8.Struct10 struct10_0, Class8.Struct4 struct4_0, Class8.Struct0 struct0_0, Class8.Struct0 struct0_1);

		// Token: 0x0600019F RID: 415
		[DllImport("libcns.dll", EntryPoint = "#281")]
		internal static extern void libcns_281(Class8.Struct10 struct10_0, Class8.Struct3 struct3_0);

		// Token: 0x060001A0 RID: 416
		[DllImport("libcns.dll", EntryPoint = "#303")]
		internal static extern void libcns_303(Class8.Struct3 struct3_0);

		// Token: 0x060001A1 RID: 417
		[DllImport("libcns.dll", EntryPoint = "#309")]
		internal static extern Class8.Struct11 libcns_309(Class8.Struct2 struct2_0, int int_0);

		// Token: 0x060001A2 RID: 418
		[DllImport("libcns.dll", EntryPoint = "#311")]
		private static extern Class8.Struct3 libcns_311(Class8.Struct11 struct11_0, int int_0, int int_1, [In] Class8.Struct1[] struct1_0);

		// Token: 0x060001A3 RID: 419 RVA: 0x00002D63 File Offset: 0x00000F63
		internal static Class8.Struct3 smethod_43(Class8.Struct11 struct11_0, int int_0, [In] Class8.Struct1[] struct1_0)
		{
			return Class8.libcns_311(struct11_0, int_0, struct1_0.Length, struct1_0);
		}

		// Token: 0x060001A4 RID: 420
		[DllImport("libcns.dll", EntryPoint = "#393")]
		internal static extern void libcns_393(Class8.Struct2 struct2_0, bool bool_0);

		// Token: 0x060001A5 RID: 421
		[DllImport("libcns.dll", EntryPoint = "#231")]
		internal static extern Class8.Struct12 libcns_231(Class8.Struct2 struct2_0);

		// Token: 0x060001A6 RID: 422
		[DllImport("libcns.dll", EntryPoint = "#233")]
		internal static extern void libcns_233(Class8.Struct12 struct12_0);

		// Token: 0x060001A7 RID: 423
		[DllImport("libcns.dll", EntryPoint = "#235")]
		internal static extern Class8.Struct14 libcns_235(Class8.Struct12 struct12_0, Class8.Struct3 struct3_0, int int_0, double double_0, Class8.Struct3 struct3_1, int int_1, double double_1);

		// Token: 0x060001A8 RID: 424
		[DllImport("libcns.dll", EntryPoint = "#319")]
		internal static extern Class8.Struct13 libcns_319(Class8.Struct4 struct4_0);

		// Token: 0x060001A9 RID: 425
		[DllImport("libcns.dll", EntryPoint = "#323")]
		internal static extern void libcns_323(Class8.Struct13 struct13_0);

		// Token: 0x060001AA RID: 426
		[DllImport("libcns.dll", EntryPoint = "#321")]
		internal static extern void libcns_321(Class8.Struct13 struct13_0, Class8.Struct3 struct3_0, int int_0, double double_0, double double_1, double double_2);

		// Token: 0x060001AB RID: 427
		[DllImport("libcns.dll", EntryPoint = "#325")]
		internal static extern Class8.Struct14 libcns_325(Class8.Struct12 struct12_0, Class8.Struct13 struct13_0, Class8.Struct3 struct3_0, int int_0, double double_0);

		// Token: 0x060001AC RID: 428
		[DllImport("libcns.dll", EntryPoint = "#389")]
		internal static extern Class8.Struct14 libcns_389(Class8.Struct12 struct12_0, Class8.Struct13 struct13_0, double double_0, double double_1);

		// Token: 0x060001AD RID: 429
		[DllImport("libcns.dll", EntryPoint = "#237")]
		internal static extern void libcns_237(Class8.Struct14 struct14_0);

		// Token: 0x060001AE RID: 430
		[DllImport("libcns.dll", EntryPoint = "#239")]
		internal static extern int libcns_239(Class8.Struct14 struct14_0);

		// Token: 0x060001AF RID: 431
		[DllImport("libcns.dll", EntryPoint = "#241")]
		internal static extern int libcns_241(Class8.Struct14 struct14_0, int int_0);

		// Token: 0x060001B0 RID: 432
		[DllImport("libcns.dll", EntryPoint = "#243")]
		internal static extern int libcns_243(Class8.Struct14 struct14_0, int int_0, int int_1);

		// Token: 0x060001B1 RID: 433
		[DllImport("libcns.dll", EntryPoint = "#245")]
		internal static extern void libcns_245(Class8.Struct14 struct14_0, int int_0, int int_1, int int_2, ref double double_0, ref double double_1);

		// Token: 0x060001B2 RID: 434
		[DllImport("libcns.dll", EntryPoint = "#327")]
		private static extern void libcns_327(Class8.Struct12 struct12_0, Class8.Struct13 struct13_0, StringBuilder stringBuilder_0);

		// Token: 0x060001B3 RID: 435 RVA: 0x00002D70 File Offset: 0x00000F70
		internal static void smethod_44(Class8.Struct12 struct12_0, Class8.Struct13 struct13_0, string string_1)
		{
			Class8.libcns_327(struct12_0, struct13_0, new StringBuilder(string_1));
		}

		// Token: 0x060001B4 RID: 436
		[DllImport("libcns.dll", EntryPoint = "#329")]
		private static extern void libcns_329(Class8.Struct14 struct14_0, StringBuilder stringBuilder_0);

		// Token: 0x060001B5 RID: 437 RVA: 0x00002D7F File Offset: 0x00000F7F
		internal static void smethod_45(Class8.Struct14 struct14_0, string string_1)
		{
			Class8.libcns_329(struct14_0, new StringBuilder(string_1));
		}

		// Token: 0x060001B6 RID: 438
		[DllImport("libcns.dll", EntryPoint = "#341")]
		internal static extern void libcns_341(Class8.Struct12 struct12_0, int int_0);

		// Token: 0x060001B7 RID: 439
		[DllImport("libcns.dll", EntryPoint = "#379")]
		internal static extern void libcns_379(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, double double_0, double double_1);

		// Token: 0x060001B8 RID: 440
		[DllImport("libcns.dll", EntryPoint = "#381")]
		internal static extern void libcns_381(Class8.Struct3 struct3_0, Class8.Struct0 struct0_0, double double_0, double double_1);

		// Token: 0x04000065 RID: 101
		private const string string_0 = "libcns.dll";

		// Token: 0x02000020 RID: 32
		internal struct Struct0
		{
			// Token: 0x04000066 RID: 102
			internal double double_0;

			// Token: 0x04000067 RID: 103
			internal double double_1;
		}

		// Token: 0x02000021 RID: 33
		internal struct Struct1
		{
			// Token: 0x04000068 RID: 104
			internal double double_0;

			// Token: 0x04000069 RID: 105
			internal double double_1;

			// Token: 0x0400006A RID: 106
			internal double double_2;
		}

		// Token: 0x02000022 RID: 34
		internal struct Struct2
		{
			// Token: 0x0400006B RID: 107
			private IntPtr intptr_0;
		}

		// Token: 0x02000023 RID: 35
		internal struct Struct3
		{
			// Token: 0x0400006C RID: 108
			internal IntPtr intptr_0;
		}

		// Token: 0x02000024 RID: 36
		internal struct Struct4
		{
			// Token: 0x0400006D RID: 109
			internal IntPtr intptr_0;
		}

		// Token: 0x02000025 RID: 37
		internal struct Struct5
		{
			// Token: 0x0400006E RID: 110
			private IntPtr intptr_0;
		}

		// Token: 0x02000026 RID: 38
		internal struct Struct6
		{
			// Token: 0x0400006F RID: 111
			private IntPtr intptr_0;
		}

		// Token: 0x02000027 RID: 39
		internal struct Struct7
		{
			// Token: 0x04000070 RID: 112
			private IntPtr intptr_0;
		}

		// Token: 0x02000028 RID: 40
		internal enum Enum1
		{
			// Token: 0x04000072 RID: 114
			const_0,
			// Token: 0x04000073 RID: 115
			const_1,
			// Token: 0x04000074 RID: 116
			const_2,
			// Token: 0x04000075 RID: 117
			const_3,
			// Token: 0x04000076 RID: 118
			const_4,
			// Token: 0x04000077 RID: 119
			const_5 = 9,
			// Token: 0x04000078 RID: 120
			const_6,
			// Token: 0x04000079 RID: 121
			const_7,
			// Token: 0x0400007A RID: 122
			const_8,
			// Token: 0x0400007B RID: 123
			const_9,
			// Token: 0x0400007C RID: 124
			const_10,
			// Token: 0x0400007D RID: 125
			const_11,
			// Token: 0x0400007E RID: 126
			const_12,
			// Token: 0x0400007F RID: 127
			const_13,
			// Token: 0x04000080 RID: 128
			const_14
		}

		// Token: 0x02000029 RID: 41
		internal enum Enum2
		{
			// Token: 0x04000082 RID: 130
			const_0,
			// Token: 0x04000083 RID: 131
			const_1,
			// Token: 0x04000084 RID: 132
			const_2,
			// Token: 0x04000085 RID: 133
			const_3,
			// Token: 0x04000086 RID: 134
			const_4,
			// Token: 0x04000087 RID: 135
			const_5
		}

		// Token: 0x0200002A RID: 42
		internal enum Enum3
		{
			// Token: 0x04000089 RID: 137
			const_0,
			// Token: 0x0400008A RID: 138
			const_1,
			// Token: 0x0400008B RID: 139
			const_2,
			// Token: 0x0400008C RID: 140
			const_3
		}

		// Token: 0x0200002B RID: 43
		internal enum Enum4
		{
			// Token: 0x0400008E RID: 142
			const_0,
			// Token: 0x0400008F RID: 143
			const_1
		}

		// Token: 0x0200002C RID: 44
		internal enum Enum5
		{
			// Token: 0x04000091 RID: 145
			const_0,
			// Token: 0x04000092 RID: 146
			const_1,
			// Token: 0x04000093 RID: 147
			const_2,
			// Token: 0x04000094 RID: 148
			const_3,
			// Token: 0x04000095 RID: 149
			const_4
		}

		// Token: 0x0200002D RID: 45
		internal enum Enum6
		{
			// Token: 0x04000097 RID: 151
			const_0,
			// Token: 0x04000098 RID: 152
			const_1,
			// Token: 0x04000099 RID: 153
			const_2,
			// Token: 0x0400009A RID: 154
			const_3
		}

		// Token: 0x0200002E RID: 46
		internal enum Enum7
		{
			// Token: 0x0400009C RID: 156
			const_0,
			// Token: 0x0400009D RID: 157
			const_1,
			// Token: 0x0400009E RID: 158
			const_2,
			// Token: 0x0400009F RID: 159
			const_3
		}

		// Token: 0x0200002F RID: 47
		internal enum Enum8
		{
			// Token: 0x040000A1 RID: 161
			const_0,
			// Token: 0x040000A2 RID: 162
			const_1,
			// Token: 0x040000A3 RID: 163
			const_2
		}

		// Token: 0x02000030 RID: 48
		internal enum Enum9
		{
			// Token: 0x040000A5 RID: 165
			const_0 = 1,
			// Token: 0x040000A6 RID: 166
			const_1,
			// Token: 0x040000A7 RID: 167
			const_2
		}

		// Token: 0x02000031 RID: 49
		internal enum Enum10
		{
			// Token: 0x040000A9 RID: 169
			const_0,
			// Token: 0x040000AA RID: 170
			const_1,
			// Token: 0x040000AB RID: 171
			const_2
		}

		// Token: 0x02000032 RID: 50
		internal struct Struct8
		{
			// Token: 0x040000AC RID: 172
			internal double double_0;

			// Token: 0x040000AD RID: 173
			internal double double_1;

			// Token: 0x040000AE RID: 174
			internal double double_2;

			// Token: 0x040000AF RID: 175
			internal double double_3;
		}

		// Token: 0x02000033 RID: 51
		internal enum Enum11
		{
			// Token: 0x040000B1 RID: 177
			const_0,
			// Token: 0x040000B2 RID: 178
			const_1,
			// Token: 0x040000B3 RID: 179
			const_2
		}

		// Token: 0x02000034 RID: 52
		internal struct Struct9
		{
			// Token: 0x060001BA RID: 442 RVA: 0x00002D8D File Offset: 0x00000F8D
			internal bool method_0()
			{
				return this.intptr_0 == IntPtr.Zero;
			}

			// Token: 0x040000B4 RID: 180
			private IntPtr intptr_0;
		}

		// Token: 0x02000035 RID: 53
		internal struct Struct10
		{
			// Token: 0x040000B5 RID: 181
			private IntPtr intptr_0;
		}

		// Token: 0x02000036 RID: 54
		internal struct Struct11
		{
			// Token: 0x040000B6 RID: 182
			private IntPtr intptr_0;
		}

		// Token: 0x02000037 RID: 55
		internal struct Struct12
		{
			// Token: 0x040000B7 RID: 183
			private IntPtr intptr_0;
		}

		// Token: 0x02000038 RID: 56
		internal struct Struct13
		{
			// Token: 0x040000B8 RID: 184
			private IntPtr intptr_0;
		}

		// Token: 0x02000039 RID: 57
		internal struct Struct14
		{
			// Token: 0x040000B9 RID: 185
			private IntPtr intptr_0;
		}
	}
}
