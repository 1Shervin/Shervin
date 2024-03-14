{
  "log": {
    "disabled": false,
    "level": "info",
    "timestamp": true
  },
  "dns": {
    "servers": [
      {
        "tag": "proxyDns",
        "address": "8.8.8.8",
        "detour": "select"
      },
      {
        "tag": "localDns",
        "address": "https://223.5.5.5/dns-query",
        "detour": "direct"
      },
      {
        "tag": "block",
        "address": "rcode://success"
      }
    ],
    "rules": [
      {
        "domain": [
          "ghproxy.com",
          "cdn.jsdelivr.net",
          "testingcf.jsdelivr.net"
        ],
        "server": "localDns"
      },
      {
        "geosite": [
          "category-ads-all"
        ],
        "server": "block"
      },
      {
        "server": "localDns",
        "outbound": "any",
        "disable_cache": true
      },
      {
        "geosite": [
          "cn"
        ],
        "server": "localDns"
      },
      {
        "server": "localDns",
        "clash_mode": "direct"
      },
      {
        "server": "proxyDns",
        "clash_mode": "global"
      },
      {
        "geosite": [
          "geolocation-!cn"
        ],
        "server": "proxyDns"
      }
    ],
    "strategy": "ipv4_only"
  },
  "inbounds": [
    {
      "sniff": true,
      "type": "mixed",
      "listen": "127.0.0.1",
      "listen_port": 1081
    },
    {
      "stack": "system",
      "auto_route": true,
      "inet4_address": "172.19.0.1/30",
      "mtu": 9000,
      "sniff": true,
      "strict_route": true,
      "type": "tun",
      "platform": {
        "http_proxy": {
          "enabled": true,
          "server": "127.0.0.1",
          "server_port": 1081
        }
      }
    }
  ],
  "outbounds": [
    {
      "tag": "select",
      "type": "selector",
      "outbounds": [
        "auto",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "auto",
      "type": "urltest",
      "outbounds": [
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ],
      "url": "https://www.gstatic.com/generate_204",
      "interval": "1m",
      "tolerance": 50
    },
    {
      "tag": "🤖 OpenAI",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🌌 Google",
      "type": "selector",
      "outbounds": [
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "📟 Telegram",
      "type": "selector",
      "outbounds": [
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🐦 Twitter",
      "type": "selector",
      "outbounds": [
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "👤 Facebook",
      "type": "selector",
      "outbounds": [
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🛍️ Amazon",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🍎 Apple",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🧩 Microsoft",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🎮 Game",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "📺 Bilibili",
      "type": "selector",
      "outbounds": [
        "direct"
      ]
    },
    {
      "tag": "🎬 MediaVideo",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🌏 !cn",
      "type": "selector",
      "outbounds": [
        "direct",
        "☬ SHΞЯVIN™_1",
        "☬ SHΞЯVIN™_2",
        "☬ SHΞЯVIN™_3",
        "☬ SHΞЯVIN™_4",
        "☬ SHΞЯVIN™_5",
        "☬ SHΞЯVIN™_6",
        "☬ SHΞЯVIN™_7",
        "☬ SHΞЯVIN™_8",
        "☬ SHΞЯVIN™_9",
        "☬ SHΞЯVIN™_10",
        "☬ SHΞЯVIN™_11",
        "☬ SHΞЯVIN™_12",
        "☬ SHΞЯVIN™_13",
        "☬ SHΞЯVIN™_14",
        "☬ SHΞЯVIN™_15",
        "☬ SHΞЯVIN™_16",
        "☬ SHΞЯVIN™_17",
        "☬ SHΞЯVIN™_18",
        "☬ SHΞЯVIN™_19",
        "☬ SHΞЯVIN™_20",
        "☬ SHΞЯVIN™_21",
        "☬ SHΞЯVIN™_22",
        "☬ SHΞЯVIN™_23",
        "☬ SHΞЯVIN™_24",
        "☬ SHΞЯVIN™_25",
        "☬ SHΞЯVIN™_26",
        "☬ SHΞЯVIN™_27",
        "☬ SHΞЯVIN™_28",
        "☬ SHΞЯVIN™_29",
        "☬ SHΞЯVIN™_30",
        "☬ SHΞЯVIN™_31",
        "☬ SHΞЯVIN™_32",
        "☬ SHΞЯVIN™_33",
        "☬ SHΞЯVIN™_34",
        "☬ SHΞЯVIN™_35",
        "☬ SHΞЯVIN™_36",
        "☬ SHΞЯVIN™_37",
        "☬ SHΞЯVIN™_38",
        "☬ SHΞЯVIN™_39",
        "☬ SHΞЯVIN™_40",
        "☬ SHΞЯVIN™_41",
        "☬ SHΞЯVIN™_42",
        "☬ SHΞЯVIN™_43",
        "☬ SHΞЯVIN™_44",
        "☬ SHΞЯVIN™_45",
        "☬ SHΞЯVIN™_46",
        "☬ SHΞЯVIN™_47",
        "☬ SHΞЯVIN™_48",
        "☬ SHΞЯVIN™_49",
        "☬ SHΞЯVIN™_50",
        "☬ SHΞЯVIN™_51",
        "☬ SHΞЯVIN™_52",
        "☬ SHΞЯVIN™_53",
        "☬ SHΞЯVIN™_54",
        "☬ SHΞЯVIN™_55",
        "☬ SHΞЯVIN™_56",
        "☬ SHΞЯVIN™_57",
        "☬ SHΞЯVIN™_58",
        "☬ SHΞЯVIN™_59",
        "☬ SHΞЯVIN™_60",
        "☬ SHΞЯVIN™_61",
        "☬ SHΞЯVIN™_62",
        "☬ SHΞЯVIN™_63",
        "☬ SHΞЯVIN™_64",
        "☬ SHΞЯVIN™_65",
        "☬ SHΞЯVIN™_66",
        "☬ SHΞЯVIN™_67",
        "☬ SHΞЯVIN™_68",
        "☬ SHΞЯVIN™_69",
        "☬ SHΞЯVIN™_70",
        "☬ SHΞЯVIN™_71",
        "☬ SHΞЯVIN™_72",
        "☬ SHΞЯVIN™_73",
        "☬ SHΞЯVIN™_74",
        "☬ SHΞЯVIN™_75",
        "☬ SHΞЯVIN™_76",
        "☬ SHΞЯVIN™_77",
        "☬ SHΞЯVIN™_78",
        "☬ SHΞЯVIN™_79",
        "☬ SHΞЯVIN™_80",
        "☬ SHΞЯVIN™_81",
        "☬ SHΞЯVIN™_82",
        "☬ SHΞЯVIN™_83",
        "☬ SHΞЯVIN™_84",
        "☬ SHΞЯVIN™_85",
        "☬ SHΞЯVIN™_86",
        "☬ SHΞЯVIN™_87",
        "☬ SHΞЯVIN™_88",
        "☬ SHΞЯVIN™_89",
        "☬ SHΞЯVIN™_90",
        "☬ SHΞЯVIN™_91",
        "☬ SHΞЯVIN™_92",
        "☬ SHΞЯVIN™_93",
        "☬ SHΞЯVIN™_94",
        "☬ SHΞЯVIN™_95",
        "☬ SHΞЯVIN™_96",
        "☬ SHΞЯVIN™_97",
        "☬ SHΞЯVIN™_98",
        "☬ SHΞЯVIN™_99",
        "☬ SHΞЯVIN™_100",
        "☬ SHΞЯVIN™_101",
        "☬ SHΞЯVIN™_102",
        "☬ SHΞЯVIN™_103",
        "☬ SHΞЯVIN™_104",
        "☬ SHΞЯVIN™_105",
        "☬ SHΞЯVIN™_106",
        "☬ SHΞЯVIN™_107",
        "☬ SHΞЯVIN™_108",
        "☬ SHΞЯVIN™_109",
        "☬ SHΞЯVIN™_110",
        "☬ SHΞЯVIN™_111",
        "☬ SHΞЯVIN™_112",
        "☬ SHΞЯVIN™_113",
        "☬ SHΞЯVIN™_114",
        "☬ SHΞЯVIN™_115",
        "☬ SHΞЯVIN™_116",
        "☬ SHΞЯVIN™_117",
        "☬ SHΞЯVIN™_118",
        "☬ SHΞЯVIN™_119",
        "☬ SHΞЯVIN™_120",
        "☬ SHΞЯVIN™_121",
        "☬ SHΞЯVIN™_122",
        "☬ SHΞЯVIN™_123",
        "☬ SHΞЯVIN™_124",
        "☬ SHΞЯVIN™_125",
        "☬ SHΞЯVIN™_126",
        "☬ SHΞЯVIN™_127",
        "☬ SHΞЯVIN™_128",
        "☬ SHΞЯVIN™_129",
        "☬ SHΞЯVIN™_130",
        "☬ SHΞЯVIN™_131",
        "☬ SHΞЯVIN™_132",
        "☬ SHΞЯVIN™_133",
        "☬ SHΞЯVIN™_134",
        "☬ SHΞЯVIN™_135",
        "☬ SHΞЯVIN™_136",
        "☬ SHΞЯVIN™_137",
        "☬ SHΞЯVIN™_138",
        "☬ SHΞЯVIN™_139",
        "☬ SHΞЯVIN™_140",
        "☬ SHΞЯVIN™_141",
        "☬ SHΞЯVIN™_142",
        "☬ SHΞЯVIN™_143",
        "☬ SHΞЯVIN™_144",
        "☬ SHΞЯVIN™_145",
        "☬ SHΞЯVIN™_146",
        "☬ SHΞЯVIN™_147",
        "☬ SHΞЯVIN™_148",
        "☬ SHΞЯVIN™_149",
        "☬ SHΞЯVIN™_150",
        "☬ SHΞЯVIN™_151",
        "☬ SHΞЯVIN™_152",
        "☬ SHΞЯVIN™_153",
        "☬ SHΞЯVIN™_154",
        "☬ SHΞЯVIN™_155",
        "☬ SHΞЯVIN™_156",
        "☬ SHΞЯVIN™_157",
        "☬ SHΞЯVIN™_158",
        "☬ SHΞЯVIN™_159",
        "☬ SHΞЯVIN™_160",
        "☬ SHΞЯVIN™_161",
        "☬ SHΞЯVIN™_162",
        "☬ SHΞЯVIN™_163",
        "☬ SHΞЯVIN™_164",
        "☬ SHΞЯVIN™_165",
        "☬ SHΞЯVIN™_166",
        "☬ SHΞЯVIN™_167",
        "☬ SHΞЯVIN™_168",
        "☬ SHΞЯVIN™_169",
        "☬ SHΞЯVIN™_170",
        "☬ SHΞЯVIN™_171",
        "☬ SHΞЯVIN™_172",
        "☬ SHΞЯVIN™_173",
        "☬ SHΞЯVIN™_174",
        "☬ SHΞЯVIN™_175",
        "☬ SHΞЯVIN™_176",
        "☬ SHΞЯVIN™_177",
        "☬ SHΞЯVIN™_178",
        "☬ SHΞЯVIN™_179",
        "☬ SHΞЯVIN™_180",
        "☬ SHΞЯVIN™_181",
        "☬ SHΞЯVIN™_182",
        "☬ SHΞЯVIN™_183",
        "☬ SHΞЯVIN™_184",
        "☬ SHΞЯVIN™_185",
        "☬ SHΞЯVIN™_186",
        "☬ SHΞЯVIN™_187",
        "☬ SHΞЯVIN™_188",
        "☬ SHΞЯVIN™_189",
        "☬ SHΞЯVIN™_190",
        "☬ SHΞЯVIN™_191",
        "☬ SHΞЯVIN™_192",
        "☬ SHΞЯVIN™_193",
        "☬ SHΞЯVIN™_194",
        "☬ SHΞЯVIN™_195",
        "☬ SHΞЯVIN™_196",
        "☬ SHΞЯVIN™_197",
        "☬ SHΞЯVIN™_198",
        "☬ SHΞЯVIN™_199",
        "☬ SHΞЯVIN™_200",
        "☬ SHΞЯVIN™_201",
        "☬ SHΞЯVIN™_202",
        "☬ SHΞЯVIN™_203",
        "☬ SHΞЯVIN™_204",
        "☬ SHΞЯVIN™_205",
        "☬ SHΞЯVIN™_206",
        "☬ SHΞЯVIN™_207",
        "☬ SHΞЯVIN™_208",
        "☬ SHΞЯVIN™_209",
        "☬ SHΞЯVIN™_210",
        "☬ SHΞЯVIN™_211",
        "☬ SHΞЯVIN™_212",
        "☬ SHΞЯVIN™_213",
        "☬ SHΞЯVIN™_214",
        "☬ SHΞЯVIN™_215",
        "☬ SHΞЯVIN™_216",
        "☬ SHΞЯVIN™_217",
        "☬ SHΞЯVIN™_218",
        "☬ SHΞЯVIN™_219",
        "☬ SHΞЯVIN™_220",
        "☬ SHΞЯVIN™_221",
        "☬ SHΞЯVIN™_222",
        "☬ SHΞЯVIN™_223",
        "☬ SHΞЯVIN™_224",
        "☬ SHΞЯVIN™_225",
        "☬ SHΞЯVIN™_226",
        "☬ SHΞЯVIN™_227",
        "☬ SHΞЯVIN™_228",
        "☬ SHΞЯVIN™_229",
        "☬ SHΞЯVIN™_230",
        "☬ SHΞЯVIN™_231",
        "☬ SHΞЯVIN™_232",
        "☬ SHΞЯVIN™_233",
        "☬ SHΞЯVIN™_234",
        "☬ SHΞЯVIN™_235",
        "☬ SHΞЯVIN™_236",
        "☬ SHΞЯVIN™_237",
        "☬ SHΞЯVIN™_238",
        "☬ SHΞЯVIN™_239",
        "☬ SHΞЯVIN™_240",
        "☬ SHΞЯVIN™_241",
        "☬ SHΞЯVIN™_242",
        "☬ SHΞЯVIN™_243",
        "☬ SHΞЯVIN™_244",
        "☬ SHΞЯVIN™_245",
        "☬ SHΞЯVIN™_246",
        "☬ SHΞЯVIN™_247",
        "☬ SHΞЯVIN™_248",
        "☬ SHΞЯVIN™_249",
        "☬ SHΞЯVIN™_250",
        "☬ SHΞЯVIN™_251",
        "☬ SHΞЯVIN™_252",
        "☬ SHΞЯVIN™_253",
        "☬ SHΞЯVIN™_254",
        "☬ SHΞЯVIN™_255",
        "☬ SHΞЯVIN™_256",
        "☬ SHΞЯVIN™_257",
        "☬ SHΞЯVIN™_258",
        "☬ SHΞЯVIN™_259",
        "☬ SHΞЯVIN™_260",
        "☬ SHΞЯVIN™_261",
        "☬ SHΞЯVIN™_262",
        "☬ SHΞЯVIN™_263",
        "☬ SHΞЯVIN™_264",
        "☬ SHΞЯVIN™_265",
        "☬ SHΞЯVIN™_266",
        "☬ SHΞЯVIN™_267",
        "☬ SHΞЯVIN™_268",
        "☬ SHΞЯVIN™_269",
        "☬ SHΞЯVIN™_270",
        "☬ SHΞЯVIN™_271",
        "☬ SHΞЯVIN™_272",
        "☬ SHΞЯVIN™_273",
        "☬ SHΞЯVIN™_274",
        "☬ SHΞЯVIN™_275",
        "☬ SHΞЯVIN™_276",
        "☬ SHΞЯVIN™_277",
        "☬ SHΞЯVIN™_278",
        "☬ SHΞЯVIN™_279",
        "☬ SHΞЯVIN™_280",
        "☬ SHΞЯVIN™_281",
        "☬ SHΞЯVIN™_282",
        "☬ SHΞЯVIN™_283",
        "☬ SHΞЯVIN™_284",
        "☬ SHΞЯVIN™_285",
        "☬ SHΞЯVIN™_286",
        "☬ SHΞЯVIN™_287",
        "☬ SHΞЯVIN™_288",
        "☬ SHΞЯVIN™_289",
        "☬ SHΞЯVIN™_290",
        "☬ SHΞЯVIN™_291",
        "☬ SHΞЯVIN™_292",
        "☬ SHΞЯVIN™_293",
        "☬ SHΞЯVIN™_294",
        "☬ SHΞЯVIN™_295",
        "☬ SHΞЯVIN™_296",
        "☬ SHΞЯVIN™_297",
        "☬ SHΞЯVIN™_298",
        "☬ SHΞЯVIN™_299",
        "☬ SHΞЯVIN™_300",
        "☬ SHΞЯVIN™_301",
        "☬ SHΞЯVIN™_302",
        "☬ SHΞЯVIN™_303",
        "☬ SHΞЯVIN™_304",
        "☬ SHΞЯVIN™_305",
        "☬ SHΞЯVIN™_306",
        "☬ SHΞЯVIN™_307",
        "☬ SHΞЯVIN™_308",
        "☬ SHΞЯVIN™_309",
        "☬ SHΞЯVIN™_310",
        "☬ SHΞЯVIN™_311",
        "☬ SHΞЯVIN™_312",
        "☬ SHΞЯVIN™_313"
      ]
    },
    {
      "tag": "🌏 cn",
      "type": "selector",
      "outbounds": [
        "direct",
        "select"
      ]
    },
    {
      "tag": "🛑 AdBlock",
      "type": "selector",
      "outbounds": [
        "block",
        "direct"
      ]
    },
    {
      "tag": "direct",
      "type": "direct"
    },
    {
      "tag": "block",
      "type": "block"
    },
    {
      "tag": "dns-out",
      "type": "dns"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_1",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_2",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_3",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_4",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_5",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_6",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_7",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_8",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_9",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_10",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_11",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_12",
      "type": "vless"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_13",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_14",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_15",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_16",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_17",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_18",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_19",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_20",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_21",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_22",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_23",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_24",
      "type": "vless"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_25",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_26",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_27",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_28",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_29",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_30",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_31",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_32",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_33",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_34",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_35",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_36",
      "type": "vless"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_37",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_38",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_39",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_40",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_41",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_42",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_43",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_44",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_45",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_46",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_47",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_48",
      "type": "vless"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_49",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_50",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_51",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_52",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_53",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_54",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_55",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_56",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_57",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_58",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_59",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_60",
      "type": "vless"
    },
    {
      "server": "15.237.245.165",
      "server_port": 22222,
      "tls": {
        "enabled": true,
        "server_name": "telegram-channel-vlessconfig.sohala.uk"
      },
      "transport": {
        "path": "/telegram-channel-vlessconfig-ws",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "05519058-d2ac-4f28-9e4a-2b2a1386749e",
      "tag": "☬ SHΞЯVIN™_61",
      "type": "vless"
    },
    {
      "server": "172.67.73.237",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "@V2ray_God=Telegram/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "7f55b425-a623-439b-bbd5-0b1778162054",
      "tag": "☬ SHΞЯVIN™_62",
      "type": "vless"
    },
    {
      "server": "104.20.224.95",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "fan.kostala.org",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "c26a65de-82bc-4997-aca7-6f1fb157f74d",
      "tag": "☬ SHΞЯVIN™_63",
      "type": "vless"
    },
    {
      "server": "85.9.108.23",
      "server_port": 51056,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "706b5622-6309-41d3-ecbb-7bc1fa209317",
      "tag": "☬ SHΞЯVIN™_64",
      "type": "vless"
    },
    {
      "server": "104.18.202.232",
      "server_port": 8880,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "69b52e77-934f-48f1-aff6-233593aaa122",
      "tag": "☬ SHΞЯVIN™_65",
      "type": "vless"
    },
    {
      "server": "193.228.91.254",
      "server_port": 22500,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/@custom_config",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "626f9b9e-ff4a-4122-9230-80180a8bc789",
      "tag": "☬ SHΞЯVIN™_66",
      "type": "vless"
    },
    {
      "server": "85.198.13.143",
      "server_port": 9103,
      "tls": {
        "enabled": true
      },
      "uuid": "3f17ff44-0d16-4d5d-a962-fa6bf33c842b",
      "tag": "☬ SHΞЯVIN™_67",
      "type": "vless"
    },
    {
      "server": "185.83.183.243",
      "server_port": 22443,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa8daf15-9ee1-4c99-a3c3-d7a02d9e65b9",
      "tag": "☬ SHΞЯVIN™_68",
      "type": "vless"
    },
    {
      "server": "31.47.45.197",
      "server_port": 32387,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2bd9c779-9b8d-4262-b317-bb7b26f6a0bc",
      "tag": "☬ SHΞЯVIN™_69",
      "type": "vless"
    },
    {
      "server": "104.21.229.172",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_70",
      "type": "vless"
    },
    {
      "server": "104.21.236.118",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_71",
      "type": "vless"
    },
    {
      "server": "104.21.236.217",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_72",
      "type": "vless"
    },
    {
      "server": "104.21.239.106",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_73",
      "type": "vless"
    },
    {
      "server": "104.21.233.18",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_74",
      "type": "vless"
    },
    {
      "server": "104.21.238.93",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_75",
      "type": "vless"
    },
    {
      "server": "104.21.230.114",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_76",
      "type": "vless"
    },
    {
      "server": "104.21.231.153",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_77",
      "type": "vless"
    },
    {
      "server": "104.21.224.78",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_78",
      "type": "vless"
    },
    {
      "server": "104.21.224.179",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_79",
      "type": "vless"
    },
    {
      "server": "104.21.233.98",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_80",
      "type": "vless"
    },
    {
      "server": "104.21.234.32",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_81",
      "type": "vless"
    },
    {
      "server": "104.21.225.203",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_82",
      "type": "vless"
    },
    {
      "server": "104.21.224.233",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_83",
      "type": "vless"
    },
    {
      "server": "104.21.229.220",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_84",
      "type": "vless"
    },
    {
      "server": "172.67.130.123",
      "server_port": 2053,
      "tls": {
        "enabled": true,
        "server_name": "solo.mmdargon.top"
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "7836cc8b-4c5b-44a5-8c31-312af9e3ebe0",
      "tag": "☬ SHΞЯVIN™_85",
      "type": "vless"
    },
    {
      "server": "104.18.69.154",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_86",
      "type": "vless"
    },
    {
      "server": "104.22.49.253",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_87",
      "type": "vless"
    },
    {
      "server": "104.18.65.196",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_88",
      "type": "vless"
    },
    {
      "server": "104.18.37.32",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_89",
      "type": "vless"
    },
    {
      "server": "104.17.19.168",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_90",
      "type": "vless"
    },
    {
      "server": "104.18.124.121",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_91",
      "type": "vless"
    },
    {
      "server": "104.17.235.113",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_92",
      "type": "vless"
    },
    {
      "server": "104.18.203.232",
      "server_port": 2087,
      "tls": {
        "enabled": true,
        "server_name": "mn.moienmusic.space"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "8054253e-4288-4ca6-916d-f40277304739",
      "tag": "☬ SHΞЯVIN™_93",
      "type": "vless"
    },
    {
      "server": "104.20.49.64",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_94",
      "type": "vless"
    },
    {
      "server": "104.17.27.210",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_95",
      "type": "vless"
    },
    {
      "server": "104.17.31.245",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_96",
      "type": "vless"
    },
    {
      "server": "104.20.53.106",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_97",
      "type": "vless"
    },
    {
      "server": "104.17.21.253",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_98",
      "type": "vless"
    },
    {
      "server": "104.17.28.21",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_99",
      "type": "vless"
    },
    {
      "server": "104.19.163.55",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_100",
      "type": "vless"
    },
    {
      "server": "104.17.135.237",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_101",
      "type": "vless"
    },
    {
      "server": "104.18.29.27",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_102",
      "type": "vless"
    },
    {
      "server": "162.159.134.234",
      "server_port": 2095,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/join--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--zedmodeon-ZEDMODEON--@zedmodeon-@ZEDMODEON--@zedmodeon-@ZEDMODEON--@zedmodeon-@ZEDMODEON?ed=1048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "a4adb1b3-9565-4403-b2a7-f8e2d79081ec",
      "tag": "☬ SHΞЯVIN™_103",
      "type": "vless"
    },
    {
      "server": "104.17.25.137",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_104",
      "type": "vless"
    },
    {
      "server": "104.26.14.85",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "tel-falcunargo-uk2.falcunar.uk.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "86cb987c-59dd-47fe-b127-c1a2ed7f96aa",
      "tag": "☬ SHΞЯVIN™_105",
      "type": "vless"
    },
    {
      "server": "104.17.24.203",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_106",
      "type": "vless"
    },
    {
      "server": "104.17.228.3",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_107",
      "type": "vless"
    },
    {
      "server": "104.18.20.156",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_108",
      "type": "vless"
    },
    {
      "server": "172.67.193.36",
      "server_port": 8880,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER-Telegram:@NUFiLTER",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "321718f9-ac26-4759-a631-1a60722f3f5d",
      "tag": "☬ SHΞЯVIN™_109",
      "type": "vless"
    },
    {
      "server": "104.18.68.215",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_110",
      "type": "vless"
    },
    {
      "server": "104.18.41.176",
      "server_port": 8080,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d716b17b-f097-49ae-8367-ae84a3760659",
      "tag": "☬ SHΞЯVIN™_111",
      "type": "vless"
    },
    {
      "server": "172.67.73.163",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "tel-falcunargo-uk2.falcunar.uk.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "86cb987c-59dd-47fe-b127-c1a2ed7f96aa",
      "tag": "☬ SHΞЯVIN™_112",
      "type": "vless"
    },
    {
      "server": "104.18.200.203",
      "server_port": 2095,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bfa53ab9-3ef9-41dc-9c9c-0aa0a45670d7",
      "tag": "☬ SHΞЯVIN™_113",
      "type": "vless"
    },
    {
      "server": "104.16.4.103",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "worker-flat-block-0d02.buxzj.workers.dev",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/TqE6jD0U75tHi0qg6pk11",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "48caea1d-1e57-4205-8dd8-dee478424f97",
      "tag": "☬ SHΞЯVIN™_114",
      "type": "vless"
    },
    {
      "server": "104.17.29.4",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_115",
      "type": "vless"
    },
    {
      "server": "104.17.25.131",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_116",
      "type": "vless"
    },
    {
      "server": "104.17.19.66",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_117",
      "type": "vless"
    },
    {
      "server": "104.17.17.249",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_118",
      "type": "vless"
    },
    {
      "server": "104.17.35.20",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_119",
      "type": "vless"
    },
    {
      "server": "104.18.121.164",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_120",
      "type": "vless"
    },
    {
      "server": "104.17.25.239",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_121",
      "type": "vless"
    },
    {
      "server": "172.66.45.153",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_122",
      "type": "vless"
    },
    {
      "server": "172.66.44.168",
      "server_port": 2096,
      "tls": {
        "enabled": true,
        "server_name": "ed9485634jkfhggh.pages.dev",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "Telegram@SINABIGO@SINABIGO@SINABIGO/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d342d11e-d424-4583-b36e-524ab1f0afa7",
      "tag": "☬ SHΞЯVIN™_123",
      "type": "vless"
    },
    {
      "server": "104.17.28.144",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_124",
      "type": "vless"
    },
    {
      "server": "104.21.40.63",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "shaliest.toptechnonews.com"
      },
      "transport": {
        "path": "/nimws",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ff3c4db3-2259-479e-a0e0-7af7d1d429db",
      "tag": "☬ SHΞЯVIN™_125",
      "type": "vless"
    },
    {
      "server": "172.67.158.249",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "knocked.aurorainiceland.com"
      },
      "transport": {
        "path": "/nimws",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "66dfb5f2-1c63-4d82-94a7-0915bedd93b9",
      "tag": "☬ SHΞЯVIN™_126",
      "type": "vless"
    },
    {
      "server": "104.18.13.130",
      "server_port": 2096,
      "tls": {
        "enabled": true,
        "server_name": "joinbezedmodeon.zedmodeon.lat",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "1dcefda8-a5f3-49b2-8c40-1f03bbe555d2",
      "tag": "☬ SHΞЯVIN™_127",
      "type": "vless"
    },
    {
      "server": "104.17.22.104",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_128",
      "type": "vless"
    },
    {
      "server": "104.17.30.209",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_129",
      "type": "vless"
    },
    {
      "server": "172.67.163.103",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "zsf-5fa.pages.dev"
      },
      "transport": {
        "path": "path/telegram@v2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d342d11e-d424-4583-b36e-524ab1f0afa4",
      "tag": "☬ SHΞЯVIN™_130",
      "type": "vless"
    },
    {
      "server": "104.17.82.198",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Telegram:@UnlimitedDev-Telegram:@UnlimitedDev-Telegram:@UnlimitedDev",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "23ad11e8-d90e-4a6f-86f8-527d211a6de1",
      "tag": "☬ SHΞЯVIN™_131",
      "type": "vless"
    },
    {
      "server": "104.17.27.50",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_132",
      "type": "vless"
    },
    {
      "server": "104.22.48.253",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_133",
      "type": "vless"
    },
    {
      "server": "104.19.146.173",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_134",
      "type": "vless"
    },
    {
      "server": "104.18.119.225",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_135",
      "type": "vless"
    },
    {
      "server": "190.93.247.155",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "slf.vip-germany.fun"
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "cd4c985f-728c-4a4b-b59d-4edfb12fc1b6",
      "tag": "☬ SHΞЯVIN™_136",
      "type": "vless"
    },
    {
      "server": "104.18.191.132",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_137",
      "type": "vless"
    },
    {
      "server": "104.17.22.239",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_138",
      "type": "vless"
    },
    {
      "server": "104.17.20.112",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_139",
      "type": "vless"
    },
    {
      "server": "104.17.31.103",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_140",
      "type": "vless"
    },
    {
      "server": "104.16.255.23",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_141",
      "type": "vless"
    },
    {
      "server": "198.41.209.190",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_142",
      "type": "vless"
    },
    {
      "server": "104.16.235.30",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "srv12.xyzquant.cloud",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/6eenmFpORi4fyf8bW",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "8ca98c98-fb0b-4007-a6e8-c8294e546763",
      "tag": "☬ SHΞЯVIN™_143",
      "type": "vless"
    },
    {
      "server": "104.18.30.217",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_144",
      "type": "vless"
    },
    {
      "server": "104.31.16.162",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_145",
      "type": "vless"
    },
    {
      "server": "104.17.16.88",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_146",
      "type": "vless"
    },
    {
      "server": "104.18.30.198",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_147",
      "type": "vless"
    },
    {
      "server": "104.18.66.207",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_148",
      "type": "vless"
    },
    {
      "server": "104.18.28.247",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_149",
      "type": "vless"
    },
    {
      "server": "104.17.25.15",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_150",
      "type": "vless"
    },
    {
      "server": "104.17.34.145",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_151",
      "type": "vless"
    },
    {
      "server": "104.17.241.75",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_152",
      "type": "vless"
    },
    {
      "server": "172.67.160.195",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_153",
      "type": "vless"
    },
    {
      "server": "104.17.23.210",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_154",
      "type": "vless"
    },
    {
      "server": "104.21.13.125",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_155",
      "type": "vless"
    },
    {
      "server": "104.21.74.139",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "monardas.aurorainiceland.com"
      },
      "transport": {
        "path": "/nimws",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce526092-81c1-42be-8354-88e58946c1f3",
      "tag": "☬ SHΞЯVIN™_156",
      "type": "vless"
    },
    {
      "server": "104.17.18.58",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_157",
      "type": "vless"
    },
    {
      "server": "104.18.200.200",
      "server_port": 2095,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bfa53ab9-3ef9-41dc-9c9c-0aa0a45670d7",
      "tag": "☬ SHΞЯVIN™_158",
      "type": "vless"
    },
    {
      "server": "172.66.213.38",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Telegram:@vp_n1-Telegram:@vp_n1-Telegram:@vp_n1-Telegram:@vp_n1-Telegram:@vp_n1-Telegram:@vp_n1",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "5d7483e9-57cd-4234-9e79-eb34d89e39f3",
      "tag": "☬ SHΞЯVIN™_159",
      "type": "vless"
    },
    {
      "server": "104.17.167.186",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_160",
      "type": "vless"
    },
    {
      "server": "104.19.172.95",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_161",
      "type": "vless"
    },
    {
      "server": "104.18.16.64",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_162",
      "type": "vless"
    },
    {
      "server": "172.66.44.168",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "ed9485634jkfhggh.pages.dev",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "Telegram@SINABIGO@SINABIGO@SINABIGO/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d342d11e-d424-4583-b36e-524ab1f0afa7",
      "tag": "☬ SHΞЯVIN™_163",
      "type": "vless"
    },
    {
      "server": "104.18.7.183",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_164",
      "type": "vless"
    },
    {
      "server": "104.17.28.225",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_165",
      "type": "vless"
    },
    {
      "server": "104.17.231.75",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_166",
      "type": "vless"
    },
    {
      "server": "104.17.17.40",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_167",
      "type": "vless"
    },
    {
      "server": "104.17.23.68",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_168",
      "type": "vless"
    },
    {
      "server": "104.18.37.8",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_169",
      "type": "vless"
    },
    {
      "server": "104.17.21.0",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_170",
      "type": "vless"
    },
    {
      "server": "104.18.3.145",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_171",
      "type": "vless"
    },
    {
      "server": "172.66.47.132",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_172",
      "type": "vless"
    },
    {
      "server": "104.18.66.85",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_173",
      "type": "vless"
    },
    {
      "server": "104.17.26.176",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_174",
      "type": "vless"
    },
    {
      "server": "104.18.30.19",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_175",
      "type": "vless"
    },
    {
      "server": "172.66.44.202",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_176",
      "type": "vless"
    },
    {
      "server": "172.67.38.130",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_177",
      "type": "vless"
    },
    {
      "server": "104.18.11.157",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_178",
      "type": "vless"
    },
    {
      "server": "104.21.69.44",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "prx11.adminwp.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "5771f2c6-4c63-4344-9db7-f23e918a2dec",
      "tag": "☬ SHΞЯVIN™_179",
      "type": "vless"
    },
    {
      "server": "104.17.21.254",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_180",
      "type": "vless"
    },
    {
      "server": "104.17.16.76",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_181",
      "type": "vless"
    },
    {
      "server": "104.17.31.8",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_182",
      "type": "vless"
    },
    {
      "server": "172.66.47.88",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "ed9485634jkfhggh.pages.dev",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "Telegram@SINABIGO@SINABIGO@SINABIGO/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d342d11e-d424-4583-b36e-524ab1f0afa7",
      "tag": "☬ SHΞЯVIN™_183",
      "type": "vless"
    },
    {
      "server": "104.18.193.243",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_184",
      "type": "vless"
    },
    {
      "server": "104.21.80.134",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "w2.sylarsun.eu.org"
      },
      "transport": {
        "path": "/?ed",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "dfb18c6f-731a-4898-a1c4-cc36c6055a90",
      "tag": "☬ SHΞЯVIN™_185",
      "type": "vless"
    },
    {
      "server": "104.18.23.64",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_186",
      "type": "vless"
    },
    {
      "server": "104.18.202.209",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "tahaquran8.xyz"
      },
      "transport": {
        "path": "/current_time",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "962a733d-2614-0b9b-7ffe-9ac92ffea8eb",
      "tag": "☬ SHΞЯVIN™_187",
      "type": "vless"
    },
    {
      "server": "104.18.71.39",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_188",
      "type": "vless"
    },
    {
      "server": "104.18.21.132",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_189",
      "type": "vless"
    },
    {
      "server": "104.22.14.250",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_190",
      "type": "vless"
    },
    {
      "server": "104.22.14.57",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_191",
      "type": "vless"
    },
    {
      "server": "104.17.105.152",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_192",
      "type": "vless"
    },
    {
      "server": "104.17.18.166",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_193",
      "type": "vless"
    },
    {
      "server": "104.18.77.35",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_194",
      "type": "vless"
    },
    {
      "server": "198.41.208.198",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_195",
      "type": "vless"
    },
    {
      "server": "104.18.67.116",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_196",
      "type": "vless"
    },
    {
      "server": "104.16.240.206",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_197",
      "type": "vless"
    },
    {
      "server": "104.18.14.99",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_198",
      "type": "vless"
    },
    {
      "server": "198.41.212.93",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_199",
      "type": "vless"
    },
    {
      "server": "104.17.20.59",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_200",
      "type": "vless"
    },
    {
      "server": "104.18.24.92",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "channel-falcunargo-de2.falcunar.uk.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "37218160-d684-4605-9f89-b5c987034969",
      "tag": "☬ SHΞЯVIN™_201",
      "type": "vless"
    },
    {
      "server": "104.17.240.149",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_202",
      "type": "vless"
    },
    {
      "server": "172.67.158.12",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "st-pl-1.brocdn.com"
      },
      "transport": {
        "path": "/websocket",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "624a4690-e06a-11ee-95c9-00505603e70d",
      "tag": "☬ SHΞЯVIN™_203",
      "type": "vless"
    },
    {
      "server": "104.18.79.173",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_204",
      "type": "vless"
    },
    {
      "server": "104.17.234.49",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_205",
      "type": "vless"
    },
    {
      "server": "104.17.22.48",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_206",
      "type": "vless"
    },
    {
      "server": "104.18.3.29",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_207",
      "type": "vless"
    },
    {
      "server": "104.17.27.104",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_208",
      "type": "vless"
    },
    {
      "server": "104.22.29.194",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_209",
      "type": "vless"
    },
    {
      "server": "104.18.22.49",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_210",
      "type": "vless"
    },
    {
      "server": "104.17.116.111",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_211",
      "type": "vless"
    },
    {
      "server": "198.41.212.215",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_212",
      "type": "vless"
    },
    {
      "server": "172.67.213.235",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "www.12reddddddd.bf"
      },
      "transport": {
        "path": "/975e3406-9ac4-45fc-a12b-30fbe810c75f",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "f69d4594-2d18-4266-abc4-eeb9c5604ca5",
      "tag": "☬ SHΞЯVIN™_213",
      "type": "vless"
    },
    {
      "server": "198.41.212.213",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_214",
      "type": "vless"
    },
    {
      "server": "190.93.247.247",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "64e2302b-2b35-482d-b1c6-672365828cbe",
      "tag": "☬ SHΞЯVIN™_215",
      "type": "vless"
    },
    {
      "server": "198.41.212.160",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_216",
      "type": "vless"
    },
    {
      "server": "190.93.244.0",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_217",
      "type": "vless"
    },
    {
      "server": "104.21.49.18",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "st-fr-1.brocdn.com"
      },
      "transport": {
        "path": "/websocket",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "3894cbc1-e06a-11ee-95c9-00505603e70d",
      "tag": "☬ SHΞЯVIN™_218",
      "type": "vless"
    },
    {
      "server": "190.93.246.247",
      "server_port": 2053,
      "tls": {
        "enabled": true,
        "server_name": "y.1lagvpn13.cfd"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "594627e3-a602-42bd-bb76-01d21921541c",
      "tag": "☬ SHΞЯVIN™_219",
      "type": "vless"
    },
    {
      "server": "172.67.204.84",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "12708050-b72c-42cb-a995-5a9e6c8928f2",
      "tag": "☬ SHΞЯVIN™_220",
      "type": "vless"
    },
    {
      "server": "104.18.124.78",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_221",
      "type": "vless"
    },
    {
      "server": "104.21.21.78",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_222",
      "type": "vless"
    },
    {
      "server": "104.18.119.227",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_223",
      "type": "vless"
    },
    {
      "server": "104.18.25.136",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_224",
      "type": "vless"
    },
    {
      "server": "104.18.67.212",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_225",
      "type": "vless"
    },
    {
      "server": "104.18.77.182",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_226",
      "type": "vless"
    },
    {
      "server": "104.18.70.238",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_227",
      "type": "vless"
    },
    {
      "server": "104.20.224.95",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "fan.kostala.org"
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ea2c6257-bb4d-4362-89c3-a2d798de40ff",
      "tag": "☬ SHΞЯVIN™_228",
      "type": "vless"
    },
    {
      "server": "104.18.77.72",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_229",
      "type": "vless"
    },
    {
      "server": "104.18.14.65",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_230",
      "type": "vless"
    },
    {
      "server": "104.18.28.20",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_231",
      "type": "vless"
    },
    {
      "server": "172.67.77.77",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_232",
      "type": "vless"
    },
    {
      "server": "104.18.71.206",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_233",
      "type": "vless"
    },
    {
      "server": "104.16.217.84",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_234",
      "type": "vless"
    },
    {
      "server": "198.41.212.180",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_235",
      "type": "vless"
    },
    {
      "server": "104.18.25.17",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_236",
      "type": "vless"
    },
    {
      "server": "172.64.146.80",
      "server_port": 8080,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "d716b17b-f097-49ae-8367-ae84a3760659",
      "tag": "☬ SHΞЯVIN™_237",
      "type": "vless"
    },
    {
      "server": "104.21.20.102",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_238",
      "type": "vless"
    },
    {
      "server": "104.18.176.46",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_239",
      "type": "vless"
    },
    {
      "server": "104.18.17.109",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_240",
      "type": "vless"
    },
    {
      "server": "104.18.12.209",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_241",
      "type": "vless"
    },
    {
      "server": "104.17.24.181",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_242",
      "type": "vless"
    },
    {
      "server": "104.17.31.104",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_243",
      "type": "vless"
    },
    {
      "server": "104.18.27.30",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_244",
      "type": "vless"
    },
    {
      "server": "172.67.152.151",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_245",
      "type": "vless"
    },
    {
      "server": "104.18.202.209",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "unlimiteddev.xn--9iqr0tm1r4wg.co",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "42e8cefd-2231-47a6-8cb0-07b17b2c54ff",
      "tag": "☬ SHΞЯVIN™_246",
      "type": "vless"
    },
    {
      "server": "104.18.37.47",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_247",
      "type": "vless"
    },
    {
      "server": "172.66.41.48",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_248",
      "type": "vless"
    },
    {
      "server": "104.18.103.37",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_249",
      "type": "vless"
    },
    {
      "server": "104.16.235.152",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_250",
      "type": "vless"
    },
    {
      "server": "104.17.211.39",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_251",
      "type": "vless"
    },
    {
      "server": "104.25.208.187",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_252",
      "type": "vless"
    },
    {
      "server": "104.21.26.209",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_253",
      "type": "vless"
    },
    {
      "server": "198.41.212.154",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_254",
      "type": "vless"
    },
    {
      "server": "188.114.97.2",
      "server_port": 8080,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "aa92655a-28e2-493e-a968-e8775d4527b4",
      "tag": "☬ SHΞЯVIN™_255",
      "type": "vless"
    },
    {
      "server": "162.159.135.234",
      "server_port": 2053,
      "tls": {
        "enabled": true,
        "server_name": "xx.1lagvpn13.cfd",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "e530ac94-d636-4d4d-84df-ecb5ed8c7fdc",
      "tag": "☬ SHΞЯVIN™_256",
      "type": "vless"
    },
    {
      "server": "104.16.5.229",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_257",
      "type": "vless"
    },
    {
      "server": "104.17.28.217",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_258",
      "type": "vless"
    },
    {
      "server": "104.24.176.7",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "hdfy6c1.freeairlaines.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "4804f14b-c1f8-452d-a6ec-eff1490aeac9",
      "tag": "☬ SHΞЯVIN™_259",
      "type": "vless"
    },
    {
      "server": "104.18.37.21",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_260",
      "type": "vless"
    },
    {
      "server": "104.17.24.37",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_261",
      "type": "vless"
    },
    {
      "server": "104.17.234.121",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_262",
      "type": "vless"
    },
    {
      "server": "172.67.204.84",
      "server_port": 8443,
      "tls": {
        "enabled": true,
        "server_name": "pa.savarkaraan.ir"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "8d458394-0caa-4ff8-8c86-74362eafc001",
      "tag": "☬ SHΞЯVIN™_263",
      "type": "vless"
    },
    {
      "server": "104.19.161.247",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_264",
      "type": "vless"
    },
    {
      "server": "198.41.212.47",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_265",
      "type": "vless"
    },
    {
      "server": "104.17.18.94",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_266",
      "type": "vless"
    },
    {
      "server": "104.18.78.132",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_267",
      "type": "vless"
    },
    {
      "server": "104.17.27.150",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_268",
      "type": "vless"
    },
    {
      "server": "104.25.31.119",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_269",
      "type": "vless"
    },
    {
      "server": "172.67.73.174",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "@V2ray_God=Telegram/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "7f55b425-a623-439b-bbd5-0b1778162054",
      "tag": "☬ SHΞЯVIN™_270",
      "type": "vless"
    },
    {
      "server": "104.17.30.201",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_271",
      "type": "vless"
    },
    {
      "server": "104.18.78.10",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_272",
      "type": "vless"
    },
    {
      "server": "104.18.203.232",
      "server_port": 2052,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2053",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "45955903-81ee-4cd3-9c8d-5c4aba2d672c",
      "tag": "☬ SHΞЯVIN™_273",
      "type": "vless"
    },
    {
      "server": "104.17.86.160",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_274",
      "type": "vless"
    },
    {
      "server": "172.67.132.209",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "bda4be04-48bf-4df1-aaf2-6d42522eab6b",
      "tag": "☬ SHΞЯVIN™_275",
      "type": "vless"
    },
    {
      "server": "104.16.39.23",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_276",
      "type": "vless"
    },
    {
      "server": "104.18.37.76",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_277",
      "type": "vless"
    },
    {
      "server": "104.18.70.98",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_278",
      "type": "vless"
    },
    {
      "server": "104.21.69.44",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7V2RAYFAST_7",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "12708050-b72c-42cb-a995-5a9e6c8928f2",
      "tag": "☬ SHΞЯVIN™_279",
      "type": "vless"
    },
    {
      "server": "104.21.51.208",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "watashi.free.de.mnhacker.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "Path/Telegram@V2ray_alpha/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ffffffff-eeae-4311-b37c-b2a67847fed2",
      "tag": "☬ SHΞЯVIN™_280",
      "type": "vless"
    },
    {
      "server": "190.93.245.142",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_281",
      "type": "vless"
    },
    {
      "server": "198.41.212.63",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_282",
      "type": "vless"
    },
    {
      "server": "198.41.208.218",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_283",
      "type": "vless"
    },
    {
      "server": "104.16.231.59",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_284",
      "type": "vless"
    },
    {
      "server": "172.67.43.55",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_285",
      "type": "vless"
    },
    {
      "server": "104.18.71.141",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_286",
      "type": "vless"
    },
    {
      "server": "172.66.44.111",
      "server_port": 2053,
      "tls": {
        "enabled": true,
        "server_name": "akfjw807r23raskodfjsf.pages.dev",
        "utls": {
          "enabled": true,
          "fingerprint": "random"
        }
      },
      "transport": {
        "path": "Telegram@SINABIGO@SINABIGO@SINABIGO/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "9bb74f9c-6385-4e90-9d16-aadf009575f8",
      "tag": "☬ SHΞЯVIN™_287",
      "type": "vless"
    },
    {
      "server": "104.22.16.171",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "god.lowswol.com",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "fc77b8b6-0096-44d2-95a4-c5fc37e04dd7",
      "tag": "☬ SHΞЯVIN™_288",
      "type": "vless"
    },
    {
      "server": "104.18.18.128",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_289",
      "type": "vless"
    },
    {
      "server": "104.18.71.158",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_290",
      "type": "vless"
    },
    {
      "server": "104.19.107.189",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_291",
      "type": "vless"
    },
    {
      "server": "23.227.38.13",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_292",
      "type": "vless"
    },
    {
      "server": "104.17.24.137",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_293",
      "type": "vless"
    },
    {
      "server": "104.17.25.82",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_294",
      "type": "vless"
    },
    {
      "server": "172.67.220.65",
      "server_port": 443,
      "tls": {
        "enabled": true,
        "server_name": "watashi.free.de.mnhacker.eu.org",
        "utls": {
          "enabled": true,
          "fingerprint": "chrome"
        }
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ffffffff-eeae-4311-b37c-b2a67847fed2",
      "tag": "☬ SHΞЯVIN™_295",
      "type": "vless"
    },
    {
      "server": "104.18.76.3",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_296",
      "type": "vless"
    },
    {
      "server": "104.21.26.145",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_297",
      "type": "vless"
    },
    {
      "server": "104.17.18.192",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_298",
      "type": "vless"
    },
    {
      "server": "104.18.202.232",
      "server_port": 2087,
      "tls": {
        "enabled": true,
        "server_name": "mn.moienmusic.space"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "8054253e-4288-4ca6-916d-f40277304739",
      "tag": "☬ SHΞЯVIN™_299",
      "type": "vless"
    },
    {
      "server": "104.17.16.87",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_300",
      "type": "vless"
    },
    {
      "server": "104.21.1.239",
      "server_port": 2083,
      "tls": {
        "enabled": true,
        "server_name": "amir2.yalda24.com"
      },
      "transport": {
        "type": "grpc"
      },
      "uuid": "db9079ad-d38e-40b0-8ab5-7b3afbe4a6ad",
      "tag": "☬ SHΞЯVIN™_301",
      "type": "vless"
    },
    {
      "server": "104.17.23.165",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_302",
      "type": "vless"
    },
    {
      "server": "104.18.69.5",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_303",
      "type": "vless"
    },
    {
      "server": "104.24.172.7",
      "server_port": 8080,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "@Maznet--@Maznet--@Maznet--@Maznet--@Maznet--@Maznet--@Maznet--@Maznet--@Maznet--@Maznet",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "2c526775-3963-4ed3-8cf5-28ea1f140b88",
      "tag": "☬ SHΞЯVIN™_304",
      "type": "vless"
    },
    {
      "server": "104.17.26.106",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_305",
      "type": "vless"
    },
    {
      "server": "104.18.120.51",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_306",
      "type": "vless"
    },
    {
      "server": "104.18.5.169",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_307",
      "type": "vless"
    },
    {
      "server": "104.17.178.219",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_308",
      "type": "vless"
    },
    {
      "server": "23.227.60.186",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_309",
      "type": "vless"
    },
    {
      "server": "104.21.22.114",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_310",
      "type": "vless"
    },
    {
      "server": "104.21.31.151",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_311",
      "type": "vless"
    },
    {
      "server": "198.41.219.52",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "435bda4c-fe5e-42c9-a3ad-15334943b38a",
      "tag": "☬ SHΞЯVIN™_312",
      "type": "vless"
    },
    {
      "server": "94.182.149.139",
      "server_port": 80,
      "tls": {
        "enabled": true
      },
      "transport": {
        "path": "/?ed=2048",
        "type": "ws",
        "max_early_data": 4096,
        "early_data_header_name": "Sec-WebSocket-Protocol"
      },
      "uuid": "ce45b6c2-13a1-4642-b227-182d9143b18c",
      "tag": "☬ SHΞЯVIN™_313",
      "type": "vless"
    }
  ],
  "route": {
    "geoip": {
      "download_url": "https://github.com/soffchen/sing-geoip/releases/latest/download/geoip.db",
      "download_detour": "select"
    },
    "geosite": {
      "download_url": "https://github.com/soffchen/sing-geosite/releases/latest/download/geosite.db",
      "download_detour": "select"
    },
    "rules": [
      {
        "protocol": "dns",
        "outbound": "dns-out"
      },
      {
        "network": "udp",
        "port": 443,
        "outbound": "block"
      },
      {
        "clash_mode": "direct",
        "outbound": "direct"
      },
      {
        "clash_mode": "global",
        "outbound": "select"
      },
      {
        "domain": [
          "v2rayse.com",
          "cfmem.com",
          "vpnse.org",
          "cff.pw",
          "tt.vg"
        ],
        "outbound": "select"
      },
      {
        "domain": [
          "clash.razord.top",
          "yacd.metacubex.one",
          "yacd.haishan.me",
          "d.metacubex.one"
        ],
        "outbound": "direct"
      },
      {
        "geosite": [
          "openai"
        ],
        "outbound": "🤖 OpenAI"
      },
      {
        "geosite": [
          "google",
          "github"
        ],
        "geoip": [
          "google"
        ],
        "outbound": "🌌 Google"
      },
      {
        "geosite": [
          "telegram"
        ],
        "geoip": [
          "telegram"
        ],
        "outbound": "📟 Telegram"
      },
      {
        "geosite": [
          "twitter"
        ],
        "geoip": [
          "twitter"
        ],
        "outbound": "🐦 Twitter"
      },
      {
        "geosite": [
          "facebook",
          "instagram"
        ],
        "geoip": [
          "facebook"
        ],
        "outbound": "👤 Facebook"
      },
      {
        "geosite": [
          "amazon"
        ],
        "outbound": "🛍️ Amazon"
      },
      {
        "geosite": [
          "apple-cn",
          "apple"
        ],
        "outbound": "🍎 Apple"
      },
      {
        "geosite": [
          "microsoft"
        ],
        "outbound": "🧩 Microsoft"
      },
      {
        "geosite": [
          "category-games"
        ],
        "outbound": "🎮 Game"
      },
      {
        "geosite": [
          "bilibili"
        ],
        "outbound": "📺 Bilibili"
      },
      {
        "geosite": [
          "tiktok",
          "netflix",
          "hbo",
          "disney",
          "primevideo"
        ],
        "geoip": [
          "netflix"
        ],
        "outbound": "🎬 MediaVideo"
      },
      {
        "geosite": [
          "geolocation-!cn"
        ],
        "outbound": "🌏 !cn"
      },
      {
        "geosite": [
          "cn"
        ],
        "geoip": [
          "private",
          "cn"
        ],
        "outbound": "🌏 cn"
      },
      {
        "geosite": [
          "category-ads-all"
        ],
        "outbound": "🛑 AdBlock"
      }
    ],
    "auto_detect_interface": true,
    "final": "select"
  },
  "experimental": {
    "clash_api": {
      "external_controller": "127.0.0.1:9090",
      "external_ui": "ui",
      "store_selected": true
    }
  }
}
