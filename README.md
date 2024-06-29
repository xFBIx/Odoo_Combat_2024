/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./*.{html,js}", "./!(build|dist|.*)/**/*.{html,js}"],
  theme: {
    extend: {
      colors: {
        "wwwrentomojocom-alabaster": "#fafafa",
        "wwwrentomojocom-nero": "#fff",
        "wwwrentomojocom-catskill-white": "#f5f7fa",
        "wwwrentomojocom-punch": "#dc3226",
        tomato: "#ff594d",
        "wwwrentomojocom-dove-gray": "#717171",
        "wwwrentomojocom-mercury": "#e6e6e6",
        "wwwrentomojocom-mine-shaft": "#313131",
        "wwwrentomojocom-black-87": "rgba(0, 0, 0, 0.87)",
        "wwwrentomojocom-black": "#000",
        "wwwrentomojocom-java": "#1dbdc0",
        lightgray: "#ccc",
        "wwwrentomojocom-boulder": "#787878",
        "wwwrentomojocom-jungle-mist": "#bfcfdc",
        "wwwrentomojocom-deco": "#c5e1a5",
      },
      spacing: {},
      fontFamily: {
        "wwwrentomojocom-inter-regular-12": "Inter",
      },
      borderRadius: {
        "base-9": "15.9px",
        "10xs": "3px",
        "8xs": "5px",
        "3xs": "10px",
      },
    },
    fontSize: {
      "sm-3": "13.3px",
      xs: "12px",
      mini: "15px",
      "xs-6": "11.6px",
      sm: "14px",
      "xs-4": "11.4px",
      "sm-9": "13.9px",
      "xs-8": "11.8px",
      "mini-1": "14.1px",
      "mini-7": "14.7px",
      "smi-6": "12.6px",
      "smi-8": "12.8px",
      "smi-7": "12.7px",
      "smi-5": "12.5px",
      "smi-9": "12.9px",
      smi: "13px",
      mid: "17px",
      "sm-8": "13.8px",
      "sm-5": "13.5px",
      inherit: "inherit",
    },
    screens: {
      mq1425: {
        raw: "screen and (max-width: 1425px)",
      },
      lg: {
        max: "1200px",
      },
      mq825: {
        raw: "screen and (max-width: 825px)",
      },
      mq450: {
        raw: "screen and (max-width: 450px)",
      },
    },
  },
  corePlugins: {
    preflight: false,
  },
};
