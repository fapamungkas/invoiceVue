<template lang="">
  <div class="w-full max-w-[1440px] mx-auto flex bg-[#F7F8FD]">
    <Sidebar />
    <!-- Main Menu -->
    <div class="flex w-full ml-[240px] h-24 flex-col">
      <!-- Application Bar components -->
      <Appbar />
      <!-- Profiles Completeness -->
      <Profiles />
      <!-- Fundamentals Information -->
      <!-- ccc -->
      <div class="w-[1240px] h-auto px-16 bg-blue-50">
        <!-- Breadcrumb -->
        <p class="py-8">
          <NuxtLink to="/admin/dashboard/invoices">Tagihan</NuxtLink> /
          <span class="font-bold"> Tagihan Logo Desain </span>
        </p>
        <!-- Button -->
        <div class="w-full bg-white my-8 h-auto rounded-lg px-10">
          <!-- Title Invoice and Button Create New Invoices -->
          <div class="flex justify-between items-center">
            <h1 class="py-6 text-heading-lg font-bold">Informasi Dasar</h1>
            <div class="h-auto w-auto flex rounded-md">
              <p class="text-[black] font-bold py-2 px-4 text-lg-bold">
                Nomor Tagihan
              </p>
              <input
                class="w-[114px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="1008"
              />
            </div>
            <!-- Nomor Tagihan -->
            <div class="flex">
              <div class="flex items-center pr-[12px]">
                <p class="text-lg-bold font-bold">Mata Uang</p>
              </div>
              <div>
                <div class="dropdown inline-block relative">
                  <button
                    class="border-[1px] border-[#C2C2C2] text-black font-semibold py-2 px-4 rounded inline-flex items-center"
                  >
                    <img src="../../../static/iconDashboard/flag.svg" alt="" />
                    &nbsp;
                    <span class="mr-1">IDR</span>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-5 w-5"
                      viewBox="0 0 20 20"
                      fill="currentColor"
                    >
                      <path
                        fill-rule="evenodd"
                        d="M10 3a1 1 0 01.707.293l3 3a1 1 0 01-1.414 1.414L10 5.414 7.707 7.707a1 1 0 01-1.414-1.414l3-3A1 1 0 0110 3zm-3.707 9.293a1 1 0 011.414 0L10 14.586l2.293-2.293a1 1 0 011.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z"
                        clip-rule="evenodd"
                      />
                    </svg>
                  </button>
                  <ul class="dropdown-menu absolute hidden text-gray-700 pt-1">
                    <li class="">
                      <a
                        class="rounded-t bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                        href="#"
                        >USD</a
                      >
                    </li>
                    <li class="">
                      <a
                        class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                        href="#"
                        >CNY</a
                      >
                    </li>
                    <li class="">
                      <a
                        class="rounded-b bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                        href="#"
                        >SAR</a
                      >
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <!-- Divider -->
          <hr class="pb-6" color="blue" width="100%" />
          <div class="flex justify-between">
            <div class="">
              <h1 class="pb-[18px] font-bold">Logo Perusahaan</h1>
              <img
                class="bg-cover"
                src="../../../static/iconDashboard/imgShort.png"
                alt=""
              />
            </div>
            <div class="ml-3">
              <h1 class="pb-[18px] font-bold">Background</h1>
              <img
                class="w-full"
                src="../../../static/iconDashboard/imgLong.png"
                alt=""
              />
            </div>
          </div>
          <!-- Nama Tagihan dan Jenis Tagihan -->
          <div class="flex pt-[32px] pb-[32px]">
            <div>
              <h1 class="font-bold text-[16px] pb-[8px]">Nama Tagihan</h1>
              <input
                class="w-[517.8px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Tagihan Logo Desain"
              />
            </div>
            <div class="pl-[16px]">
              <h1 class="font-bold text-[16px] pb-[8px]">Jenis Tagihan</h1>
              <div class="">
                <div class="dropdown inline-block relative">
                  <button
                    class="justify-between w-[517.4px] border-[1px] border-[#C2C2C2] text-black font-semibold py-2 px-4 rounded inline-flex items-center"
                  >
                    <div>
                      <span class="mr-1">Tagihan Satuan</span>
                    </div>
                    <div>
                      <svg
                        xmlns="http://www.w3.org/2000/svg"
                        class="h-5 w-5"
                        viewBox="0 0 20 20"
                        fill="currentColor"
                      >
                        <path
                          fill-rule="evenodd"
                          d="M10 3a1 1 0 01.707.293l3 3a1 1 0 01-1.414 1.414L10 5.414 7.707 7.707a1 1 0 01-1.414-1.414l3-3A1 1 0 0110 3zm-3.707 9.293a1 1 0 011.414 0L10 14.586l2.293-2.293a1 1 0 011.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z"
                          clip-rule="evenodd"
                        />
                      </svg>
                    </div>
                  </button>
                  <ul
                    class="dropdown-menu absolute hidden text-gray-700 pt-1 w-[517.4px]"
                  >
                    <li class="">
                      <a
                        class="rounded-t bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                        href="#"
                        >USD</a
                      >
                    </li>
                    <li class="">
                      <a
                        class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                        href="#"
                        >CNY</a
                      >
                    </li>
                  </ul>
                </div>
              </div>
            </div>
            <!-- Durasi Project dan Batas Tagihan -->
          </div>
          <div class="flex pb-10">
            <div>
              <div>
                <h1 class="text-lg-regular font-bold pb-[8px]">
                  Durasi Projek
                </h1>
                <div class="flex justify-between">
                  <input
                    class="w-[250px] border border-[#C2C2C2] py-2 px-4 rounded-[4px]"
                    type="date"
                    value="2021-06-12"
                  />
                  <input
                    class="w-[250px] border-[1px] border-[#C2C2C2] py-2 px-4 rounded-[4px] ml-[16px]"
                    type="date"
                    value="2021-06-01"
                  />
                </div>
              </div>
            </div>
            <div class="pl-[2px]">
              <h1 class="text-lg-regular font-bold pb-[8px] pl-4">
                Batas Awal Tagihan
              </h1>
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] py-2 px-4 rounded-[4px] ml-[16px]"
                type="date"
                value="2021-06-01"
              />
            </div>
            <div>
              <h1 class="text-lg-regular font-bold pb-[8px] pl-4">
                Batas Akhir Tagihan
              </h1>
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] py-2 px-4 rounded-[4px] ml-[16px]"
                type="date"
                value="2021-06-12"
              />
            </div>
          </div>
        </div>
        <!-- Kolom Dua -->
        <div class="w-full bg-white my-8 h-auto rounded-lg px-10">
          <!-- Title Invoice and Button Create New Invoices -->
          <div class="flex justify-between items-center">
            <h1 class="py-6 text-heading-lg font-bold">Tagihan Pekerjaan</h1>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="flex text-[14px] pb-[26px] font-bold">
            <h1 class="pl-[72px]">Keterangan Pekerjaan</h1>
            <h1 class="pl-[127px]">Qty</h1>
            <h1 class="pl-[150px]">Tarif</h1>
            <h1 class="pl-[285px]">Jumlah</h1>
          </div>
          <hr class="pb-6" color="solid blue" width="100%" />
          <div class="flex">
            <div class="my-auto">
              <img
                class="pl-6"
                src="../../../static/iconDashboard/dots.png"
                alt=""
              />
            </div>
            <div class="pl-[26px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Logo Desain - Paket Basic"
              />
            </div>
            <div class="pl-[16px]">
              <input
                class="w-[150px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="1"
              />
            </div>
            <div class="pl-[16px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="5.000.000"
              />
            </div>
            <div class="w-[192px] pl-[16px] text-right my-auto">
              <h1>IDR 5.000.000,00</h1>
            </div>
            <div class="pl-[70px]">
              <img class="" src="../../../static/detail/dangerRed.png" alt="" />
            </div>
          </div>
          <div class="pl-[70px] pt-5">
            <textarea
              class="border border-[#C2C2C2] rounded px-1 py-1"
              id="w3review"
              name="w3review"
              rows="3"
              cols="26"
            >
  Tuliskan deskripsi pekerjaan disini...
            </textarea>
          </div>
          <div class="pl-[70px] pt-5 pb-20">
            <button
              class="flex bg-[#F7F8FD] hover:bg-[#202E63] text-[#405DC7] hover:text-white font-bold py-2 px-[46px] rounded"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-6 w-6"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
                />
              </svg>
              &nbsp; Tambah Pekerjaan
            </button>
          </div>
          <div class="flex text-md-bold font-bold pb-7">
            <div class="pl-[72px]">
              <h1>Biaya Tambahan</h1>
            </div>
            <div class="pl-[277px]">
              <h1>Persentase</h1>
            </div>
            <div class="pl-[310px]">
              <h1>Jumlah</h1>
            </div>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="grid grid-cols-3 pl-[72px]">
            <div class="my-auto">
              <h1>Diskon</h1>
            </div>
            <div class="pl-[50px]">
              <input
                class="w-[114px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="0 %"
              />
            </div>
            <div class="pl-32">
              <h1>-</h1>
            </div>
          </div>
          <div class="pt-7">
            <div class="grid grid-cols-3 pl-[72px]">
              <div class="my-auto">
                <h1>Pajak</h1>
              </div>
              <div class="pl-[50px]">
                <input
                  class="w-[114px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                  type="text"
                  id="fname"
                  name="fname"
                  value="0 %"
                />
              </div>
              <div class="pl-32">
                <h1>-</h1>
              </div>
            </div>
          </div>
          <div class="text-sm font-bold pl-[72px] pt-7 flex justify-between">
            <div>
              <h1>Total</h1>
            </div>
            <div class="pr-32">
              <h1>IDR 5.000.000,00</h1>
            </div>
          </div>
          <div
            class="text-sm font-bold pl-[72px] pt-7 pb-6 flex justify-between"
          >
            <h2>Jangka Waktu Pembayaran</h2>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="flex text-md-bold font-bold pb-7">
            <div class="pl-[72px]">
              <h1>Keterangan Pekerjaan</h1>
            </div>
            <div class="pl-[246px]">
              <h1>Persentase</h1>
            </div>
            <div class="pl-[310px]">
              <h1>Jumlah</h1>
            </div>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="flex pb-7">
            <div class="my-auto">
              <img
                class="pl-6"
                src="../../../static/iconDashboard/dots.png"
                alt=""
              />
            </div>
            <div class="pl-[26px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Down Payment (DP)"
              />
            </div>
            <div class="pl-[130px]">
              <input
                class="w-[114px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="50%"
              />
            </div>
            <div class="my-auto pl-[260px]">
              <h1>IDR 5.000.000,00</h1>
            </div>
            <div class="pl-[58px]">
              <img class="" src="../../../static/detail/dangerRed.png" alt="" />
            </div>
          </div>
          <div>
            <div class="pl-[56px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] py-2 px-4 rounded-[4px] ml-[16px]"
                type="date"
                value="2021-06-12"
              />
            </div>
          </div>
          <div class="pt-6">
            <hr class="pb-6" color="blue" width="100%" />
          </div>
          <div class="flex pb-7">
            <div class="my-auto">
              <img
                class="pl-6"
                src="../../../static/iconDashboard/dots.png"
                alt=""
              />
            </div>
            <div class="pl-[26px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Second Term"
              />
            </div>
            <div class="pl-[130px]">
              <input
                class="w-[114px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="25%"
              />
            </div>
            <div class="my-auto pl-[260px]">
              <h1>IDR 1.250.000,00</h1>
            </div>
            <div class="pl-[58px]">
              <img class="" src="../../../static/detail/dangerRed.png" alt="" />
            </div>
          </div>
          <div>
            <div class="pl-[56px]">
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] py-2 px-4 rounded-[4px] ml-[16px]"
                type="date"
                value="2021-06-12"
              />
            </div>
          </div>
          <div class="pl-[70px] pt-9 pb-20">
            <button
              class="flex bg-[#F7F8FD] hover:bg-[#202E63] text-[#405DC7] hover:text-white font-bold py-2 px-[32px] rounded"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-6 w-6"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
                />
              </svg>
              &nbsp; Tambah Jangka Waktu
            </button>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="pb-10">
            <h2 class="font-bold">Catatan Untuk Klien</h2>
            <div class="pt-5">
              <textarea
                class="border border-[#C2C2C2] text-[#757575] p-2 rounded"
                id="w3review"
                name="w3review"
                rows="6"
                cols="121"
              >
 Tuliskan catatan anda disini...
            </textarea
              >
            </div>
          </div>
        </div>
        <!-- Kolom Tagihan Pekerjaan -->
        <div class="w-full bg-white my-8 h-auto rounded-lg px-10 pb-10">
          <!-- Title Invoice and Button Create New Invoices -->
          <div class="flex justify-between items-center">
            <h1 class="py-6 text-heading-lg font-bold">Metode Pembayaran</h1>
          </div>
          <hr class="pb-6" color="blue" width="100%" />
          <div class="border border-[#D7DDF4] rounded-[8px]">
            <div>
              <h2 class="text-lg font-bold leading-[150%] pl-28 py-10">
                Transfer Bank
              </h2>
            </div>
            <div class="pl-28">
              <h2>Pilih Layanan Bank:</h2>
              <div class="dropdown inline-block relative pt-4">
                <button
                  class="justify-between w-[900px] border-[1px] border-[#C2C2C2] text-black font-semibold py-2 px-4 rounded inline-flex items-center"
                >
                  <div>
                    <span class="mr-1 text-[#757575]">Pilih Pembayaran</span>
                  </div>
                  <div>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-5 w-5"
                      viewBox="0 0 20 20"
                      fill="currentColor"
                    >
                      <path
                        fill-rule="evenodd"
                        d="M10 3a1 1 0 01.707.293l3 3a1 1 0 01-1.414 1.414L10 5.414 7.707 7.707a1 1 0 01-1.414-1.414l3-3A1 1 0 0110 3zm-3.707 9.293a1 1 0 011.414 0L10 14.586l2.293-2.293a1 1 0 011.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z"
                        clip-rule="evenodd"
                      />
                    </svg>
                  </div>
                </button>
                <ul
                  class="dropdown-menu absolute hidden text-gray-700 pt-1 w-[900px]"
                >
                  <li class="">
                    <a
                      class="rounded-t bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                      href="#"
                      >USD</a
                    >
                  </li>
                  <li class="">
                    <a
                      class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                      href="#"
                      >CNY</a
                    >
                  </li>
                </ul>
              </div>
              <div class="grid grid-cols-2 pt-4">
                <div>
                  <h2>Nomor rekening:</h2>
                </div>
                <div>
                  <h2>Nama Pemilik:</h2>
                </div>
              </div>
              <div class="grid grid-cols-2 py-4">
                <div>
                  <div class="">
                    <input
                      class="w-[420px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px] text-[#757575]"
                      type="text"
                      id="fname"
                      name="fname"
                      value="Tuliskan nomor rekening anda"
                    />
                  </div>
                </div>
                <div>
                  <div class="">
                    <input
                      class="w-[420px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px] text-[#757575]"
                      type="text"
                      id="fname"
                      name="fname"
                      value="Tuliskan nama pemilik akun"
                    />
                  </div>
                </div>
              </div>
              <hr class="" color="blue" width="95%" />
              <div>
                <div class="py-4">
                  <h2>Pilih Layanan Bank:</h2>
                  <div class="dropdown inline-block relative pt-4">
                    <button
                      class="justify-between w-[900px] border-[1px] border-[#C2C2C2] text-black font-semibold py-2 px-4 rounded inline-flex items-center"
                    >
                      <div>
                        <span class="mr-1 text-[#757575]"
                          >Pilih Pembayaran</span
                        >
                      </div>
                      <div>
                        <svg
                          xmlns="http://www.w3.org/2000/svg"
                          class="h-5 w-5"
                          viewBox="0 0 20 20"
                          fill="currentColor"
                        >
                          <path
                            fill-rule="evenodd"
                            d="M10 3a1 1 0 01.707.293l3 3a1 1 0 01-1.414 1.414L10 5.414 7.707 7.707a1 1 0 01-1.414-1.414l3-3A1 1 0 0110 3zm-3.707 9.293a1 1 0 011.414 0L10 14.586l2.293-2.293a1 1 0 011.414 1.414l-3 3a1 1 0 01-1.414 0l-3-3a1 1 0 010-1.414z"
                            clip-rule="evenodd"
                          />
                        </svg>
                      </div>
                    </button>
                    <ul
                      class="dropdown-menu absolute hidden text-gray-700 pt-1 w-[900px]"
                    >
                      <li class="">
                        <a
                          class="rounded-t bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                          href="#"
                          >USD</a
                        >
                      </li>
                      <li class="">
                        <a
                          class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                          href="#"
                          >CNY</a
                        >
                      </li>
                    </ul>
                  </div>
                  <div class="grid grid-cols-2 pt-4">
                    <div>
                      <h2>Nomor rekening:</h2>
                    </div>
                    <div>
                      <h2>Nama Pemilik:</h2>
                    </div>
                  </div>
                  <div class="grid grid-cols-2 py-4">
                    <div>
                      <div class="">
                        <input
                          class="w-[420px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px] text-[#757575]"
                          type="text"
                          id="fname"
                          name="fname"
                          value="Tuliskan nomor rekening anda"
                        />
                      </div>
                    </div>
                    <div>
                      <div class="">
                        <input
                          class="w-[420px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px] text-[#757575]"
                          type="text"
                          id="fname"
                          name="fname"
                          value="Tuliskan nama pemilik akun"
                        />
                      </div>
                    </div>
                  </div>
                </div>
                <div class="pt-9 pb-10">
                  <button
                    class="flex bg-[#F7F8FD] hover:bg-[#202E63] text-[#405DC7] hover:text-white font-bold py-2 px-[32px] rounded"
                  >
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="h-6 w-6"
                      fill="none"
                      viewBox="0 0 24 24"
                      stroke="currentColor"
                    >
                      <path
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
                      />
                    </svg>
                    &nbsp; Tambah Pembayaran Baru
                  </button>
                </div>
              </div>
            </div>
          </div>
          <div class="border border-[#D7DDF4] rounded-[8px] mt-8">
            <div>
              <h2 class="text-lg text-[#404040] font-bold pl-28 py-8">
                PayPal Akun
              </h2>
            </div>
            <div class="pl-28 text-[#757575]">
              <h2>Masukkan Email PayPal Anda:</h2>
            </div>
            <div class="pl-28 pt-4 pb-10">
              <input
                class="w-[900px] border-[1px] bg-[#EDEDED] border-[#C2C2C2] rounded py-[8px] px-[16px] text-[#757575]"
                type="text"
                id="fname"
                name="fname"
                value="Tuliskan Email PayPal Anda"
              />
            </div>
          </div>
        </div>
        <div class="w-full bg-white my-8 h-auto rounded-lg px-10 pb-10">
          <!-- Title Invoice and Button Create New Invoices -->
          <div class="flex justify-between items-center">
            <h1 class="py-6 text-heading-lg font-bold">Pengaturan Tagihan</h1>
          </div>
          <hr class="" color="blue" width="100%" />
          <div class="flex justify-between pt-8">
            <div>
              <h2 class="font-bold">Pilih Tema Untuk Tagihan</h2>
            </div>
            <div>
              <a href="">
                <h2 class="text-sm font-bold text-[#405DC7] underline">
                  Lihat semua tema
                </h2>
              </a>
            </div>
          </div>
          <div class="w-full flex justify-between text-center text-[#757575]">
            <div>
              <img
                class="pl-6"
                src="../../../static/detail/groupSatu.png"
                alt=""
              />
              <h2>Matternhorn</h2>
            </div>
            <div class="">
              <img
                class="pl-6"
                src="../../../static/detail/groupDua.png"
                alt=""
              />
              <h2>Jungfrao</h2>
            </div>
            <div>
              <img
                class="pl-6"
                src="../../../static/detail/groupTiga.png"
                alt=""
              />
              <h2>Patternaw</h2>
            </div>
            <div>
              <img
                class="pl-6"
                src="../../../static/detail/groupEmpat.png"
                alt=""
              />
              <h2>Brutal</h2>
            </div>
            <div>
              <img
                class="pl-6"
                src="../../../static/detail/groupLima.png"
                alt=""
              />
              <h2>Schiltorm</h2>
            </div>
          </div>
          <div class="pt-8">
            <hr class="mx-auto" color="blue" width="90%" />
          </div>
          <div class="flex justify-between text-lg text-left py-8">
            <div>
              <h2 class="font-bold pb-1">Tagihan untuk:</h2>
              <div class="text-[#0A0A0A]">
                <h2 class="py-1">Udin Alexander</h2>
                <h2 class="py-1">Sample Company LLC</h2>
                <h2 class="py-1">Client Address, NY 12345</h2>
                <h2 class="py-1">Udin.a@sample.com</h2>
              </div>
            </div>
            <div>
              <h2 class="font-bold">Penerbit Tagihan:</h2>
              <h2 class="pt-4 pb-1">Nama Penerbit</h2>
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Fay Miftachus"
              />
              <h2 class="pt-4 pb-1">Jabatan Penerbit</h2>
              <input
                class="w-[250px] border-[1px] border-[#C2C2C2] rounded py-[8px] px-[16px]"
                type="text"
                id="fname"
                name="fname"
                value="Account Manager"
              />
            </div>
            <div>
              <h2 class="font-bold">Pengingat Tagihan</h2>
              <div class="flex pt-4">
                <div class="">
                  <h2>
                    Apakah anda ingin <br />
                    pengingat untuk tagihan ini?
                  </h2>
                </div>
              </div>
            </div>
            <div>
              <div class="30%">
                <img
                  class="w-[50%] pt-10"
                  src="../../../static/detail/On.png"
                  alt=""
                />
              </div>
            </div>
          </div>
          <hr color="blue" width="100%" />
          <div class="pt-8 pb-6">
            <h2 class="text-lg font-bold">Lampiran</h2>
          </div>
          <div>
            <a href="">
              <img
                class="w-[100%]"
                src="../../../static/detail/addLampiran.png"
                alt=""
              />
            </a>
          </div>
        </div>
        <!-- Kolom Tinjau dan Kirim -->
        <div class="flex justify-end pb-20">
          <div class="pr-6">
            <button
              class="flex bg-white hover:bg-blue-700 text-black hover:text-white font-bold py-2 px-4 rounded"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-5 w-5"
                viewBox="0 0 20 20"
                fill="currentColor"
              >
                <path
                  fill-rule="evenodd"
                  d="M4 4a2 2 0 012-2h4.586A2 2 0 0112 2.586L15.414 6A2 2 0 0116 7.414V16a2 2 0 01-2 2H6a2 2 0 01-2-2V4zm2 6a1 1 0 011-1h6a1 1 0 110 2H7a1 1 0 01-1-1zm1 3a1 1 0 100 2h6a1 1 0 100-2H7z"
                  clip-rule="evenodd"
                />
              </svg>
              &ensp; Simpan Sebagai Draft
            </button>
          </div>
          <div>
            <button
              class="flex bg-[#405DC7] hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="h-5 w-5 rotate-45"
                viewBox="0 0 20 20"
                fill="currentColor"
              >
                <path
                  d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"
                />
              </svg>
              &ensp; Tinjau & Kirim
            </button>
          </div>
        </div>
      </div>

      <script>
        export default {
          name: "InvoiceLogo",
          head: {
            title: "Timvoice - Tagihan Logo",
            meta: [
              {
                charset: "utf-8",
              },
              {
                name: "viewport",
                content: "width=device-width, initial-scale=1",
              },
              {
                hid: "invoice tagihan logo",
                name: "invoice product - tagihan page logo",
                content: "invoice product - tagihan logo",
              },
            ],
            link: [
              {
                rel: "icon",
                type: "image/x-icon",
                href: "/favicon.ico",
              },
              {
                rel: "stylesheets",
                href: "https://fonts.googleapis.com/css2?family=Mulish:wght@400;500;600;700;800&display=swap",
              },
            ],
          },
        };
      </script>
      <style>
        .dropdown:hover .dropdown-menu {
          display: block;
        }
      </style>
    </div>

    <script>
      export default {
        name: "InvoiceLogo",
        head: {
          title: "Timvoice - Tagihan Logo",
          meta: [
            {
              charset: "utf-8",
            },
            {
              name: "viewport",
              content: "width=device-width, initial-scale=1",
            },
            {
              hid: "invoice tagihan logo",
              name: "invoice product - tagihan page logo",
              content: "invoice product - tagihan logo",
            },
          ],
          link: [
            {
              rel: "icon",
              type: "image/x-icon",
              href: "/favicon.ico",
            },
            {
              rel: "stylesheets",
              href: "https://fonts.googleapis.com/css2?family=Mulish:wght@400;500;600;700;800&display=swap",
            },
          ],
        },
      };
    </script>
    <style>
      .dropdown:hover .dropdown-menu {
        display: block;
      }
    </style>
  </div>
</template>

<script>
export default {
  name: "InvoiceLogo",
  head: {
    title: "Timvoice - Tagihan Logo",
    meta: [
      {
        charset: "utf-8",
      },
      {
        name: "viewport",
        content: "width=device-width, initial-scale=1",
      },
      {
        hid: "invoice tagihan logo",
        name: "invoice product - tagihan page logo",
        content: "invoice product - tagihan logo",
      },
    ],
    link: [
      {
        rel: "icon",
        type: "image/x-icon",
        href: "/favicon.ico",
      },
      {
        rel: "stylesheets",
        href: "https://fonts.googleapis.com/css2?family=Mulish:wght@400;500;600;700;800&display=swap",
      },
    ],
  },
};
</script>
<style>
.dropdown:hover .dropdown-menu {
  display: block;
}
</style>
