# Reference

A reference article is information-oriented.
It provides a structured description of a product:
its APIs, classes, functions, configuration options, actions, and so on.
Start with a summary of what this reference article is about, and what the items you are describing are used for.

## Command

작업예정

Application():
CellShape():
CellShapeprop):
CharShape():
CharShapeprop):
CLSID():
coclass_clsid():
CurFieldState():
CurMetatagState():
CurSelectedCtrl():
EditMode():
EditModeprop):
EngineProperties():
HAction():
HeadCtrl():
HParameterSet():
IsEmpty() -> bool:
IsModified() -> bool:
IsPrivateInfoProtected():
IsTrackChangePassword():
IsTrackChange():
LastCtrl():
PageCount():
ParaShape():
ParaShapeprop):
ParentCtrl():
Path():
SelectionMode():
Version():
ViewProperties():
ViewPropertiesprop):
XHwpDocuments():
XHwpMessageBox():
XHwpODBC():
XHwpWindows():
ctrl_list():
current_page():
current_printpage():
current_font():
get_linespacingmethod: Literal["Fixed", "Percent", "BetweenLines", "AtLeast"] = "Percent") -> int:
set_linespacingvalue:int=160, method:Literal["Fixed", "Percent", "BetweenLines", "AtLeast"] = "Percent") -> int:
is_empty_para():
goto_addraddr: str|int = "A1", col: int=0, select: bool=False):
get_field_info():
get_image_infoctrl):
goto_stylestyle: Union[int, str]):
get_into_table_caption():
shape_copy_pasteType: Literal["font", "para", "both"] = "both", cell_attr: bool = False,
export_mathmlmml_path, delay=0.2):
import_mathmlmml_path, delay=0.2):
maximize_window():
minimize_window():
delete_style_by_namesrc: int | str, dst: int | str):
get_style_dictas_: list | dict = None):
get_style():
set_stylestyle: int|str):
get_selected_range():
fill_addr_field():
unfill_addr_field():
resize_imagewidth: int = None, height: int = None, unit: Literal["mm", "hwpunit"] = "mm"):
save_imagepath="./img.png", ctrl=""):
NewNumberModifynew_number: int,
NewNumbernew_number: int,
PageNumPosglobal_start: int = 1, position: Literal[
table_to_stringrowsep="", colsep="\r\n"):
extract_content_from_table(sep):
set_cell_marginleft: float = 1.8, right: float = 1.8, top: float = 0.5, bottom: float = 0.5, as_: Literal["mm", "hwpunit"] = "mm") -> bool:
get_cell_marginas_: Literal["mm", "hwpunit"] = "mm") -> Union[dict, bool]:
set_table_inside_marginleft: float = 1.8, right: float = 1.8, top: float = 0.5, bottom: float = 0.5, as_: Literal["mm", "hwpunit"] = "mm") -> bool:
get_table_inside_marginas_: Literal["mm", "hwpunit"] = "mm") -> Union[dict, bool]:
get_table_outside_marginas_: Literal["mm", "hwpunit"] = "mm") -> Union[dict, bool]:
get_table_outside_margin_leftas_: Literal["mm", "hwpunit"] = "mm"):
get_table_outside_margin_rightas_: Literal["mm", "hwpunit"] = "mm"):
get_table_outside_margin_topas_: Literal["mm", "hwpunit"] = "mm"):
get_table_outside_margin_bottomas_: Literal["mm", "hwpunit"] = "mm"):
set_table_outside_marginleft: float = 1.0, right: float = 1.0, top: float = 1.0, bottom: float = 1.0, as_: Literal["mm", "hwpunit"] = "mm") -> bool:
set_table_outside_margin_leftval, as_: Literal["mm", "hwpunit"] = "mm"):
set_table_outside_margin_rightval, as_: Literal["mm", "hwpunit"] = "mm"):
set_table_outside_margin_topval, as_: Literal["mm", "hwpunit"] = "mm"):
set_table_outside_margin_bottomval, as_: Literal["mm", "hwpunit"] = "mm"):
get_table_heightas_: Literal["mm", "hwpunit", "point", "inch"] = "mm"):
get_row_num():
get_row_heightas_: Literal["mm", "hwpunit", "point", "inch"] = "mm"):
get_col_num():
get_col_widthas_: Literal["mm", "hwpunit", "point", "inch"] = "mm"):
set_col_widthwidth: int | float | list | tuple, as_: Literal["mm", "ratio"] = "ratio"):
adjust_cellwidthwidth: int | float | list | tuple, as_: Literal["mm", "ratio"] = "ratio"):
get_table_widthas_: Literal["mm", "hwpunit", "point", "inch"] = "mm"):
set_table_widthwidth: int = 0, as_: Literal["mm", "hwpunit", "hu"] = "mm"):
save_pdf_as_imagepath: str = "", img_format="bmp"):
get_cell_addras_: Literal["str", "tuple"] = "str"):
save_all_picturessave_path="./binData"):
select_ctrlctrl, anchor_type: Literal[0, 1, 2] = 0):
move_to_ctrlctrl):
set_visiblevisible):
auto_spacinginit_spacing=0, init_ratio=100, max_spacing=40, min_spacing=40, verbose=True):
reset_para_spacing(init_spacing=init_spacing, init_ratio=init_ratio):
get_spacing_dir():
select_spacing_area(direction=0):
modify_spacing(direction=0):
set_font(,
cell_fillface_color: tuple[int, int, int] = (217, 217, 217)):
fields_to_dict():
get_into_nth_tablen=0, select=False):
set_row_heightheight: int | float, as_: Literal["mm", "hwpunit"] = "mm"):
remove_background_picture():
gradation_on_cellcolor_list: list[tuple] | list[str] = [(0, 0, 0), (255, 255, 255)],
get_available_font() -> list:
get_charshape():
get_charshape_as_dict():
set_charshapepset):
get_markpen_color():
get_pagedef():
get_pagedef_as_dictas_: Literal["kor", "eng"] = "kor"):
set_pagedefpset, apply: Literal["cur", "all", "new"] = "cur"):
save_block_aspath, format="HWP", attributes=1):
goto_printpagepage_num: int = 1):
goto_pagepage_index: int | str = 1) -> tuple[int, int]:
table_from_datadata, transpose=False, header0="", treat_as_char=False, header=True, index=True,
countword):
delete_all_fields():
delete_field_by_namefield_name, idx=-1):
markpen_on_selectionr=255, g=255, b=0):
open_pdfpdf_path, this_window=1):
msgboxstring, flag: int = 0):
insert_filefilename, keep_section=1, keep_charshape=1, keep_parashape=1, keep_style=1,
insert_memotext, memo_type: Literal["revision", "memo"] = "memo"):
is_cell():
find_backwardsrc, regex=False):
find_forwardsrc, regex=False):
findsrc, direction: Literal["Forward", "Backward", "AllDoc"] = "Forward", regex=False, MatchCase=1,
set_field_by_bracket():
find_replacesrc, dst, regex=False, direction: Literal["Backward", "Forward", "AllDoc"] = "Forward",
find_replace_allsrc, dst, regex=False, MatchCase=1, AllWordForms=0, SeveralWords=1, UseWildCards=1,
clipboard_to_pyfunc():
clear_field_text():
switch_tonum):
add_tab():
add_doc():
hwp_unit_to_milihwp_unit):
HwpUnitToMilihwp_unit: int) -> float:
create_tablerows, cols, treat_as_char: bool = True, width_type=0, height_type=0, header=True, height=0):
get_selected_textas_: Literal["list", "str"] = "str"):
table_to_csvn="", filename="result.csv", encoding="utf-8", startrow=0):
table_to_df_qn="", startrow=0, columns=[]):
table_to_dfn="", cols=0, selected_range=None, start_pos=None):
table_to_bottomoffset=0.):
insert_texttext):
insert_lorempara_num=1):
move_all_captionlocation: Literal["Top", "Bottom", "Left", "Right"] = "Bottom",
is_empty() -> bool:
is_modified() -> bool:
arc_typearc_type):
ArcTypearc_type):
auto_num_typeautonum):
AutoNumTypeautonum):
border_shapeborder_type):
BorderShapeborder_type):
break_word_latinbreak_latin_word):
BreakWordLatinbreak_latin_word):
brush_typebrush_type):
BrushTypebrush_type):
canonicalcanonical):
Canonicalcanonical):
cell_applycell_apply):
CellApplycell_apply):
char_shadow_typeshadow_type):
CharShadowTypeshadow_type):
check_xobjectbstring):
CheckXObjectbstring):
clearoption: int = 1):
Clearoption: int = 1):
closeis_dirty: bool = False, interval=0.01):
col_def_typecol_def_type):
ColDefTypecol_def_type):
col_layout_typecol_layout_type):
ColLayoutTypecol_layout_type):
convert_pua_hangul_to_unicodereverse):
ConvertPUAHangulToUnicodereverse):
create_actionactidstr: str):
CreateActionactidstr: str):
create_fieldname: str, direction: str = "", memo: str = "") -> bool:
CreateFieldname: str, direction: str = "", memo: str = "") -> bool:
create_idcreation_id):
CreateIdcreation_id):
create_modecreation_mode):
CreateModecreation_mode):
create_page_imagepath: str, pgno: int = -1, resolution: int = 300, depth: int = 24,
CreatePageImagepath: str, pgno: int = -1, resolution: int = 300, depth: int = 24,
create_setsetidstr):
CreateSetsetidstr):
crooked_slashcrooked_slash):
CrookedSlashcrooked_slash):
ds_markdiac_sym_mark):
DSMarkdiac_sym_mark):
dbf_code_typedbf_code):
DbfCodeTypedbf_code):
delete_ctrlctrl) -> bool:
DeleteCtrlctrl) -> bool:
DeleteDocumentMasterPage():
DeleteSectionMasterPage():
delimiterdelimiter):
Delimiterdelimiter):
draw_aspectdraw_aspect):
DrawAspectdraw_aspect):
draw_fill_imagefillimage):
DrawFillImagefillimage):
draw_shadow_typeshadow_type):
DrawShadowTypeshadow_type):
encryptencrypt):
Encryptencrypt):
end_sizeend_size):
EndSizeend_size):
end_styleend_style):
EndStyleend_style):
EquationCreatethread=False):
EquationClosesave=False, delay=0.1):
EquationModifythread=False):
EquationRefresh():  # , delay=0.2):
export_stylesty_filepath: str) -> bool:
ExportStylesty_filepath: str) -> bool:
field_existfield):
FieldExistfield):
file_translatecur_lang, trans_lang):
FileTranslatecur_lang, trans_lang):
fill_area_typefill_area):
FillAreaTypefill_area):
find_ctrl():
FindCtrl():
find_dirfind_dir: Literal["Forward", "Backward", "AllDoc"] = "AllDoc"):
FindDirfind_dir: Literal["Forward", "Backward", "AllDoc"] = "AllDoc"):
find_private_infoprivate_type, private_string):
FindPrivateInfoprivate_type, private_string):
font_typefont_type):
FontTypefont_type):
get_bin_data_pathbinid):
GetBinDataPathbinid):
get_cur_field_nameoption=0):
GetCurFieldNameoption=0):
get_cur_metatag_name():
GetCurMetatagName():
get_field_listnumber=1, option=0):
GetFieldListnumber=1, option=0):
get_field_textfield: str | list | tuple | set, idx=0):
GetFieldTextfield: str | list | tuple | set, idx=0):
get_file_infofilename):
GetFileInfofilename):
get_font_listlangid=""):
GetFontListlangid=""):
get_heading_string():
GetHeadingString():
get_message_box_mode():
GetMessageBoxMode():
get_metatag_listnumber, option):
GetMetatagListnumber, option):
get_metatag_name_texttag):
GetMetatagNameTexttag):
get_mouse_posx_rel_to=1, y_rel_to=1):
GetMousePosx_rel_to=1, y_rel_to=1):
get_page_textpgno: int = 0, option: hex = 0xffffffff) -> str:
GetPageTextpgno: int = 0, option: hex = 0xffffffff) -> str:
get_pos() -> tuple[int]:
GetPos() -> tuple[int]:
get_pos_by_set():
GetPosBySet():
get_script_sourcefilename: str) -> str:
GetScriptSourcefilename: str) -> str:
get_selected_pos():
GetSelectedPos():
get_selected_pos_by_setsset, eset):
GetSelectedPosBySetsset, eset):
get_text():
GetText():
get_text_fileformat="UNICODE", option=""):
GetTextFileformat="UNICODE", option=""):
get_translate_lang_listcur_lang):
GetTranslateLangListcur_lang):
get_user_infouser_info_id):
GetUserInfouser_info_id):
gradationgradation):
Gradationgradation):
grid_methodgrid_method):
GridMethodgrid_method):
grid_view_linegrid_view_line):
GridViewLinegrid_view_line):
gutter_methodgutter_type):
GutterMethodgutter_type):
h_alignh_align):
HAlignh_align):
handlerhandler):
Handlerhandler):
hashhash):
Hashhash):
hatch_stylehatch_style):
HatchStylehatch_style):
head_typeheading_type):
HeadTypeheading_type):
height_relheight_rel):
HeightRelheight_rel):
hidinghiding):
Hidinghiding):
horz_relhorz_rel):
HorzRelhorz_rel):
hwp_line_typeline_type: Literal[
HwpLineTypeline_type: Literal[
hwp_line_widthline_width: Literal[
HwpLineWidthline_width: Literal[
hwp_outline_stylehwp_outline_style):
HwpOutlineStylehwp_outline_style):
hwp_outline_typehwp_outline_type):
HwpOutlineTypehwp_outline_type):
hwp_underline_shapehwp_underline_shape):
HwpUnderlineShapehwp_underline_shape):
hwp_underline_typehwp_underline_type):
HwpUnderlineTypehwp_underline_type):
hwp_zoom_typezoom_type):
HwpZoomTypezoom_type):
image_formatimage_format):
ImageFormatimage_format):
import_stylesty_filepath):
ImportStylesty_filepath):
init_hparameter_set():
InitHParameterSet():
init_scanoption=0x07, range=0x77, spara=0, spos=0, epara=-1, epos=-1):
InitScanoption=0x07, range=0x77, spara=0, spos=0, epara=-1, epos=-1):
insertpath, format="", arg="", move_doc_end=False):
insert_background_picturepath,
InsertBackgroundPicturepath, border_type: Literal["SelectedCell", "SelectedCellDelete"] = "SelectedCell",
insert_ctrlctrl_id, initparam):
InsertCtrlctrl_id, initparam):
insert_picturepath, treat_as_char=True, embedded=True, sizeoption=0, reverse=False, watermark=False,
insert_picturepath, treat_as_char=True, embedded=True, sizeoption=0, reverse=False, watermark=False,
insert_random_picturex: int = 200, y: int = 200):
is_action_enableaction_id):
IsActionEnableaction_id):
is_command_lockaction_id):
IsCommandLockaction_id):
key_indicator() -> tuple:
KeyIndicator() -> tuple:
line_spacing_methodline_spacing):
LineSpacingMethodline_spacing):
line_wrap_typeline_wrap):
LineWrapTypeline_wrap):
lock_commandact_id, is_lock):
LockCommandact_id, is_lock):
lunar_to_solarl_year, l_month, l_day, l_leap, s_year, s_month, s_day):
LunarToSolarl_year, l_month, l_day, l_leap, s_year, s_month, s_day):
lunar_to_solar_by_setl_year, l_month, l_day, l_leap):
LunarToSolarBySetl_year, l_month, l_day, l_leap):
macro_statemacro_state):
MacroStatemacro_state):
mail_typemail_type):
MailTypemail_type):
MarkPenNext():
MarkPenPrev():
metatag_existtag):
MetatagExisttag):
mili_to_hwp_unitmili):
MiliToHwpUnitmili):
modify_field_propertiesfield, remove, add):
ModifyFieldPropertiesfield, remove, add):
modify_metatag_propertiestag, remove, add):
ModifyMetatagPropertiestag, remove, add):
move_posmove_id=1, para=0, pos=0):
MovePosmove_id=1, para=0, pos=0):
move_to_fieldfield, idx=0, text=True, start=True, select=False):
MoveToFieldfield, idx=0, text=True, start=True, select=False):
move_to_metatagtag, text, start, select):
MoveToMetatagtag, text, start, select):
number_formatnum_format):
NumberFormatnum_format):
numberingnumbering):
Numberingnumbering):
openfilename, format="", arg=""):
Openfilename, format="", arg=""):
page_num_positionpagenumpos: Literal[
PageNumPositionpagenumpos: Literal[
page_typepage_type):
PageTypepage_type):
para_head_alignpara_head_align):
ParaHeadAlignpara_head_align):
pic_effectpic_effect):
PicEffectpic_effect):
placement_typerestart):
PlacementTyperestart):
point_to_hwp_unitpoint):
PointToHwpUnitpoint):
hwp_unit_to_pointHwpUnit: int):
HwpUnitToPointHwpUnit: int):
hwp_unit_to_inchHwpUnit):
HwpUnitToInchHwpUnit):
inch_to_hwp_unitinch):
InchToHwpUnitinch):
present_effectprsnteffect):
PresentEffectprsnteffect):
print_deviceprint_device):
PrintDeviceprint_device):
print_paperprint_paper):
PrintPaperprint_paper):
print_rangeprint_range):
PrintRangeprint_range):
print_typeprint_method):
PrintTypeprint_method):
protect_private_infoprotecting_char, private_pattern_type):
ProtectPrivateInfoprotecting_char, private_pattern_type):
put_field_textfield, text: Union[str, list, tuple, pd.Series] = "", idx=None):
PutFieldTextfield, text: Union[str, list, tuple, pd.Series] = "", idx=None):
put_metatag_name_texttag, text):
PutMetatagNameTexttag, text):
quit():
Quit():
rgb_colorred_or_colorname: str | tuple, green=255, blue=255):
RGBColorred_or_colorname: str | tuple, green=255, blue=255):
register_modulemodule_type="FilePathCheckDLL", module_data="FilePathCheckerModule"):
RegisterModulemodule_type="FilePathCheckDLL", module_data="FilePathCheckerModule"):
register_regedit():
register_private_info_patternprivate_type, private_pattern):
RegisterPrivateInfoPatternprivate_type, private_pattern):
release_actionaction):
ReleaseActionaction):
release_scan():
ReleaseScan():
rename_fieldoldname, newname):
rename_metatagoldtag, newtag):
RenameMetatagoldtag, newtag):
replace_actionold_action_id, new_action_id):
ReplaceActionold_action_id, new_action_id):
replace_fontlangid, des_font_name, des_font_type, new_font_name, new_font_type):
ReplaceFontlangid, des_font_name, des_font_type, new_font_name, new_font_type):
revisionrevision):
Revisionrevision):
Runact_id):
ASendBrowserText():
AutoChangeHangul():
AutoChangeRun():
AutoSpellRun():
AutoSpellSelect0():
AutoSpellSelect1():
AutoSpellSelect2():
AutoSpellSelect3():
AutoSpellSelect4():
AutoSpellSelect5():
AutoSpellSelect6():
AutoSpellSelect7():
AutoSpellSelect8():
AutoSpellSelect9():
AutoSpellSelect10():
AutoSpellSelect11():
AutoSpellSelect12():
AutoSpellSelect13():
AutoSpellSelect14():
AutoSpellSelect15():
AutoSpellSelect16():
BottomTabFrameClose():
BreakColDef():
BreakColumn():
BreakLine():
BreakPage():
BreakPara():
BreakSection():
Cancel():
CaptureHandler():
CaptureDialog():
ChangeSkin():
CharShapeBold():
CharShapeCenterline():
CharShapeEmboss():
CharShapeEngrave():
CharShapeHeight():
CharShapeHeightDecrease():
CharShapeHeightIncrease():
CharShapeItalic():
CharShapeLang():
CharShapeNextFaceName():
CharShapeNormal():
CharShapeOutline():
CharShapePrevFaceName():
CharShapeShadow():
CharShapeSpacing():
CharShapeSpacingDecrease():
CharShapeSpacingIncrease():
CharShapeSubscript():
CharShapeSuperscript():
CharShapeSuperSubscript():
CharShapeTextColorBlack():
CharShapeTextColorBlue():
CharShapeTextColorBluish():
CharShapeTextColorGreen():
CharShapeTextColorRed():
CharShapeTextColorViolet():
CharShapeTextColorWhite():
CharShapeTextColorYellow():
CharShapeTypeface():
CharShapTypeface():
CharShapeUnderline():
CharShapeWidth():
CharShapeWidthDecrease():
CharShapeWidthIncrease():
Close():
CloseEx():
Comment():
CommentDelete():
CommentModify():
ComposeCharsChars: str | int = "", CharSize: int = -3, CheckCompose: int = 0, CircleType: int = 0,
Copy():
CopyPage():
CustCopyBtn():
CustCutBtn():
CustEraseBtn():
CustInsSepBtn():
CustomizeToolbar():
CustPasteBtn():
CustRenameBtn():
CustRestBtn():
CustViewIconBtn():
CustViewIconNameBtn():
CustViewNameBtn():
Cutremove_cell=True):
Deletedelete_ctrl=True):
DeleteBackdelete_ctrl=True):
DeleteField():
DeleteFieldMemo():
DeleteLinedelete_ctrl=True):
DeleteLineEnddelete_ctrl=True):
DeletePage():
DeleteWorddelete_ctrl=True):
DeleteWordBackdelete_ctrl=True):
DrawObjCancelOneStep():
DrawObjEditDetail():
DrawObjOpenClosePolygon():
DrawObjTemplateSave():
EasyFind():
EditFieldMemo():
Erase():
FileClose():
FileFind():
FileNew():
FileNewTab():
FileNextVersionDiff():
FilePrevVersionDiff():
FileOpen():
FileOpenMRU():
FilePreview():
FileQuit():
FileSave():
FileSaveAs():
FileSaveAsDRM():
FileVersionDiffChangeAlign():
FileVersionDiffSameAlign():
FileVersionDiffSyncScroll():
FillColorShadeDec():
FillColorShadeInc():
FindForeBackBookmark():
FindForeBackCtrl():
FindForeBackFind():
FindForeBackLine():
FindForeBackPage():
FindForeBackSection():
FindForeBackSelectCtrl():
FindForeBackStyle():
FormDesignMode():
FormObjCreatorCheckButton():
FormObjCreatorComboBox():
FormObjCreatorEdit():
FormObjCreatorPushButton():
FormObjCreatorRadioButton():
FormObjRadioGroup():
FrameFullScreen():
FrameFullScreenEnd():
FrameHRuler():
FrameStatusBar():
FrameViewZoomRibon():
FrameVRuler():
HancomRoom():
HanThDIC():
HeaderFooterDelete():
HeaderFooterModify():
HeaderFooterToNext():
HeaderFooterToPrev():
HelpContents():
HelpIndex():
HelpWeb():
HiddenCredits():
HideTitle():
HimConfig():
HimKbdChange():
HorzScrollbar():
HwpCtrlEquationCreate97():
HwpCtrlFileNew():
HwpCtrlFileOpen():
HwpCtrlFileSave():
HwpCtrlFileSaveAs():
HwpCtrlFileSaveAsAutoBlock():
HwpCtrlFileSaveAutoBlock():
HwpCtrlFindDlg():
HwpCtrlReplaceDlg():
HwpDic():
HwpTabViewAction():
HwpTabViewAttribute():
HwpTabViewClipboard():
HwpTabViewDistant():
HwpTabViewHwpDic():
HwpTabViewMasterPage():
HwpTabViewOutline():
HwpTabViewScript():
HwpViewType():
HwpWSDic():
HyperlinkBackward():
HyperlinkForward():
ImageFindPath():
InputCodeChange():
InputHanja():
InputHanjaBusu():
InputHanjaMean():
InsertAutoNum():
InsertCpNo():
InsertCpTpNo():
InsertDateCode():
InsertDocInfo():
InsertEndnote():
InsertFieldDateTime():
InsertFieldMemo():
InsertFieldRevisionChagne():
InsertFixedWidthSpace():
InsertFootnote():
InsertLastPrintDate():
InsertLastSaveBy():
InsertLastSaveDate():
InsertLine():
InsertNonBreakingSpace():
InsertPageNum():
InsertSoftHyphen():
InsertSpace():
InsertStringDateTime():
InsertTab():
InsertTpNo():
Jajun():
LabelAdd():
LabelTemplate():
LeftShiftBlock():
LeftTabFrameClose():
LinkTextBox():
MacroPause():
MacroPlay1():
MacroPlay10():
MacroPlay11():
MacroPlay2():
MacroPlay3():
MacroPlay4():
MacroPlay5():
MacroPlay6():
MacroPlay7():
MacroPlay8():
MacroPlay9():
MacroRepeat():
MacroStop():
MailMergeField():
MakeIndex():
ManualChangeHangul():
MarkPenColor():
MarkTitle():
MasterPage():
MasterPageDuplicate():
MasterPageExcept():
MasterPageFront():
MasterPagePrevSection():
MasterPageToNext():
MasterPageToPrevious():
MasterPageType():
MasterWsItemOnOff():
ModifyComposeChars():
ModifyCtrl():
ModifyDutmal():
ModifyFillProperty():
ModifyLineProperty():
ModifyShapeObject():
MoveColumnBegin():
MoveColumnEnd():
MoveDocBegin():
MoveDocEnd():
MoveDown():
MoveLeft():
MoveLineBegin():
MoveLineDown():
MoveLineEnd():
MoveLineUp():
MoveListBegin():
MoveListEnd():
MoveNextChar():
MoveNextColumn():
MoveNextParaBegin():
MoveNextPos():
MoveNextPosEx():
MoveNextWord():
MovePageBegin():
MovePageDown():
MovePageEnd():
MovePageUp():
MoveParaBegin():
MoveParaEnd():
MoveParentList():
MovePrevChar():
MovePrevColumn():
MovePrevParaBegin():
MovePrevParaEnd():
MovePrevPos():
MovePrevPosEx():
MovePrevWord():
MoveRight():
MoveRootList():
MoveScrollDown():
MoveScrollNext():
MoveScrollPrev():
MoveScrollUp():
MoveSectionDown():
MoveSectionUp():
MoveSelDocBegin():
MoveSelDocEnd():
MoveSelDown():
MoveSelLeft():
MoveSelLineBegin():
MoveSelLineDown():
MoveSelLineEnd():
MoveSelLineUp():
MoveSelListBegin():
MoveSelListEnd():
MoveSelNextChar():
MoveSelNextParaBegin():
MoveSelNextPos():
MoveSelNextWord():
MoveSelPageDown():
MoveSelPageUp():
MoveSelParaBegin():
MoveSelParaEnd():
MoveSelPrevChar():
MoveSelPrevParaBegin():
MoveSelPrevParaEnd():
MoveSelPrevPos():
MoveSelPrevWord():
MoveSelRight():
MoveSelTopLevelBegin():
MoveSelTopLevelEnd():
MoveSelUp():
MoveSelViewDown():
MoveSelViewUp():
MoveSelWordBegin():
MoveSelWordEnd():
MoveTopLevelBegin():
MoveTopLevelEnd():
MoveTopLevelList():
MoveUp():
MoveViewBegin():
MoveViewDown():
MoveViewEnd():
MoveViewUp():
MoveWordBegin():
MoveWordEnd():
MPSectionToNext():
MPSectionToPrevious():
NextTextBoxLinked():
NoteDelete():
NoSplit():
NoteLineColor():
NoteLineLength():
NoteLineShape():
NoteLineWeight():
NoteModify():
NoteNumProperty():
NoteNumShape():
NotePosition():
NoteToNext():
NoteToPrev():
ParagraphShapeAlignCenter():
ParagraphShapeAlignDistribute():
ParagraphShapeAlignDivision():
ParagraphShapeAlignJustify():
ParagraphShapeAlignLeft():
ParagraphShapeAlignRight():
ParagraphShapeDecreaseLeftMargin():
ParagraphShapeDecreaseLineSpacing():
ParagraphShapeDecreaseMargin():
ParagraphShapeDecreaseRightMargin():
ParagraphShapeIncreaseLeftMargin():
ParagraphShapeIncreaseLineSpacing():
ParagraphShapeIncreaseMargin():
ParagraphShapeIncreaseRightMargin():
ParagraphShapeIndentAtCaret():
ParagraphShapeIndentNegative():
ParagraphShapeIndentPositive():
ParagraphShapeProtect():
ParagraphShapeWithNext():
ParaShapeLineSpace():
pasteoption: Literal[0, 1, 2, 3, 4, 5, 6] = 4):
Paste():
PastePage():
PasteSpecial():
PictureEffect1():
PictureEffect2():
PictureEffect3():
PictureEffect4():
PictureEffect5():
PictureEffect6():
PictureEffect7():
PictureEffect8():
PictureInsertDialog():
PictureLinkedToEmbedded():
PictureSave():
PictureScissor():
PictureToOriginal():
PrevTextBoxLinked():
PstAutoPlay():
PstBlackToWhite():
PstGradientType():
PstScrChangeType():
PstSetupNextSec():
PstSetupPrevSec():
QuickCommandRun():
QuickCorrect():
QuickCorrectRun():
QuickCorrectSound():
QuickMarkInsert0():
QuickMarkInsert1():
QuickMarkInsert2():
QuickMarkInsert3():
QuickMarkInsert4():
QuickMarkInsert5():
QuickMarkInsert6():
QuickMarkInsert7():
QuickMarkInsert8():
QuickMarkInsert9():
QuickMarkMove0():
QuickMarkMove1():
QuickMarkMove2():
QuickMarkMove3():
QuickMarkMove4():
QuickMarkMove5():
QuickMarkMove6():
QuickMarkMove7():
QuickMarkMove8():
QuickMarkMove9():
RecalcPageCount():
RecentCode():
RecentEmpty():
RecentNoExistDel():
Redo():
returnKeyInField():
ReturnKeyInField():
returnPrevPos():
ReturnPrevPos():
RightShiftBlock():
RightTabFrameClose():
RunUserKeyLayout():
ScrMacroPause():
ScrMacroPlay1():
ScrMacroPlay2():
ScrMacroPlay3():
ScrMacroPlay4():
ScrMacroPlay5():
ScrMacroPlay6():
ScrMacroPlay7():
ScrMacroPlay8():
ScrMacroPlay9():
ScrMacroPlay10():
ScrMacroPlay11():
ScrMacroRepeat():
ScrMacroStop():
Select():
SelectAll():
SelectColumn():
SelectCtrlFront():
SelectCtrlReverse():
SendBrowserText():
SetWorkSpaceView():
ShapeObjAlignBottom():
ShapeObjAlignCenter():
ShapeObjAlignHeight():
ShapeObjAlignHorzSpacing():
ShapeObjAlignLeft():
ShapeObjAlignMiddle():
ShapeObjAlignRight():
ShapeObjAlignSize():
ShapeObjAlignTop():
ShapeObjAlignVertSpacing():
ShapeObjAlignWidth():
ShapeObjAttachCaption():
ShapeObjAttachTextBox():
ShapeObjBringForward():
ShapeObjBringInFrontOfText():
ShapeObjBringToFront():
ShapeObjCtrlSendBehindText():
ShapeObjDetachCaption():
ShapeObjDetachTextBox():
ShapeObjFillProperty():
ShapeObjGroup():
ShapeObjHorzFlip():
ShapeObjHorzFlipOrgState():
ShapeObjInsertCaptionNum():
ShapeObjLineProperty():
ShapeObjLock():
ShapeObjMoveDown():
ShapeObjMoveLeft():
ShapeObjMoveRight():
ShapeObjMoveUp():
ShapeObjNextObject():
ShapeObjNorm():
ShapeObjPrevObject():
ShapeObjResizeDown():
ShapeObjResizeLeft():
ShapeObjResizeRight():
ShapeObjResizeUp():
ShapeObjRightAngleRotater():
ShapeObjRightAngleRotaterAnticlockwise():
ShapeObjRotater():
ShapeObjSaveAsPicture():
ShapeObjSelect():
ShapeObjSendBack():
ShapeObjSendToBack():
ShapeObjTableSelCell():
ShapeObjTextBoxEdit():
ShapeObjUngroup():
ShapeObjUnlockAll():
ShapeObjVertFlip():
ShapeObjVertFlipOrgState():
ShapeObjWrapSquare():
ShapeObjWrapTopAndBottom():
ShowAttributeTab():
ShowBottomWorkspace():
ShowFloatTabFrame():
ShowLeftWorkspace():
ShowRightWorkspace():
ShowScriptTab():
ShowTopWorkspace():
SoftKeyboard():
SpellingCheck():
SplitAll():
SplitHorz():
SplitMainActive():
SplitMemo():
SplitMemoClose():
SplitMemoOpen():
SplitVert():
StyleClearCharStyle():
StyleCombo():
StyleShortcut1():
StyleShortcut2():
StyleShortcut3():
StyleShortcut4():
StyleShortcut5():
StyleShortcut6():
StyleShortcut7():
StyleShortcut8():
StyleShortcut9():
StyleShortcut10():
TabClose():
TableAppendRow():
TableAutoFill():
TableAutoFillDlg():
TableCellAlignCenterBottom():
TableCellAlignCenterCenter():
TableCellAlignCenterTop():
TableCellAlignLeftBottom():
TableCellAlignLeftCenter():
TableCellAlignLeftTop():
TableCellAlignRightBottom():
TableCellAlignRightCenter():
TableCellAlignRightTop():
TableCellBlock():
TableCellBlockCol():
TableCellBlockExtend():
TableCellBlockExtendAbs():
TableCellBlockRow():
TableCellBorderAll():
TableCellBorderBottom():
TableCellBorderDiagonalDown():
TableCellBorderDiagonalUp():
TableCellBorderInside():
TableCellBorderInsideHorz():
TableCellBorderInsideVert():
TableCellBorderLeft():
TableCellBorderNo():
TableCellBorderOutside():
TableCellBorderRight():
TableCellBorderTop():
TableColBegin():
TableColEnd():
TableColPageDown():
TableColPageUp():
TableDeleteCellremain_cell=False):
TableDistributeCellHeight():
TableDistributeCellWidth():
TableDrawPen():
TableDrawPenStyle():
TableDrawPenWidth():
TableEraser():
TableFormulaAvgAuto():
TableFormulaAvgHor():
TableFormulaAvgVer():
TableFormulaProAuto():
TableFormulaProHor():
TableFormulaProVer():
TableFormulaSumAuto():
TableFormulaSumHor():
TableFormulaSumVer():
TableLeftCell():
TableLowerCell():
TableMergeCell():
TableMergeTable():
TableResizeCellDown():
TableResizeCellLeft():
TableResizeCellRight():
TableResizeCellUp():
TableResizeDown():
TableResizeExDown():
TableResizeExLeft():
TableResizeExRight():
TableResizeExUp():
TableResizeLeft():
TableResizeLineDown():
TableResizeLineLeft():
TableResizeLineRight():
TableResizeLineUp():
TableResizeRight():
TableResizeUp():
TableRightCell():
TableRightCellAppend():
TableSplitCellRows=2, Cols=0, DistributeHeight=0, Merge=0):
TableSplitTable():
TableUpperCell():
TableVAlignBottom():
TableVAlignCenter():
TableVAlignTop():
ToggleOverwrite():
TopTabFrameClose():
Undo():
UnlinkTextBox():
VersionDeleteAll():
VertScrollbar():
ViewIdiom():
ViewOptionCtrlMark():
ViewOptionGuideLine():
ViewOptionMemo():
ViewOptionMemoGuideline():
ViewOptionPaper():
ViewOptionParaMark():
ViewOptionPicture():
ViewOptionRevision():
ViewTabButton():
ViewZoomFitPage():
ViewZoomNormal():
ViewZoomFitWidth():
ViewZoomRibon():
VoiceCommandConfig():
VoiceCommandResume():
VoiceCommandStop():
run_script_macrofunction_name, u_macro_type=0, u_script_type=0):
RunScriptMacrofunction_name, u_macro_type=0, u_script_type=0):
savesave_if_dirty=True):
Savesave_if_dirty=True):
save_aspath, format="HWP", arg="", split_page=False):
press_key(hexKeyCode):
release_key(hexKeyCode):
find_window_and_send_key(window_name, key_code, retries=5, delay=0.1):
find_window_and_confirm(window_name, retries=5, delay=0.1):
save_as_html_plus(path, visible=True):
SaveAspath, format="HWP", arg=""):
scan_font():
ScanFont():
select_text_by_get_poss_getpos, e_getpos):
select_textspara: Union[int, list, tuple] = 0, spos=0, epara=0, epos=0, slist=0):
SelectTextspara: Union[int, list, tuple] = 0, spos=0, epara=0, epos=0, slist=0):
set_bar_code_imagelp_image_path, pgno, index, x, y, width, height):
SetBarCodeImagelp_image_path, pgno, index, x, y, width, height):
set_cur_field_namefield, option=0, direction="", memo=""):
SetCurFieldNamefield, option=0, direction="", memo=""):
set_cur_metatag_nametag):
SetCurMetatagNametag):
set_drm_authorityauthority):
SetDRMAuthorityauthority):
set_field_view_optionoption):
SetFieldViewOptionoption):
set_message_box_modemode):
SetMessageBoxModemode):
set_poslist, para, pos):
SetPoslist, para, pos):
set_pos_by_setdisp_val):
SetPosBySetdisp_val):
set_private_info_passwordpassword):
SetPrivateInfoPasswordpassword):
set_text_filedata: str, format: Literal["HWP", "HWPML2X", "HTML", "UNICODE", "TEXT"] = "HWPML2X",
SetTextFiledata: str, format: Literal["HWP", "HWPML2X", "HTML", "UNICODE", "TEXT"] = "HWPML2X",
set_title_nametitle):
SetTitleNametitle):
set_user_infouser_info_id, value):
SetUserInfouser_info_id, value):
side_typeside_type):
SideTypeside_type):
signaturesignature):
Signaturesignature):
slashslash):
Slashslash):
solar_to_lunars_year, s_month, s_day, l_year, l_month, l_day, l_leap):
SolarToLunars_year, s_month, s_day, l_year, l_month, l_day, l_leap):
solar_to_lunar_by_sets_year, s_month, s_day):
SolarToLunarBySets_year, s_month, s_day):
sort_delimitersort_delimiter):
SortDelimitersort_delimiter):
strike_outstrike_out_type):
StrikeOutstrike_out_type):
style_typestyle_type):
StyleTypestyle_type):
subt_possubt_pos):
SubtPossubt_pos):
table_breakpage_break):
TableBreakpage_break):
table_formattable_format):
TableFormattable_format):
table_swap_typetableswap):
TableSwapTypetableswap):
table_targettable_target):
TableTargettable_target):
text_aligntext_align):
TextAligntext_align):
text_art_aligntext_art_align):
TextArtAligntext_art_align):
text_dirtext_direction):
TextDirtext_direction):
text_flow_typetext_flow):
TextFlowTypetext_flow):
text_wrap_typetext_wrap):
TextWrapTypetext_wrap):
un_select_ctrl():
UnSelectCtrl():
v_alignv_align):
VAlignv_align):
vert_relvert_rel):
VertRelvert_rel):
view_flagview_flag):
ViewFlagview_flag):
watermark_brushwatermark_brush):
WatermarkBrushwatermark_brush):
width_relwidth_rel):
WidthRelwidth_rel):
WindowAlignCascade():
WindowAlignTileHorz():
WindowAlignTileVert():
WindowList():
WindowMinimizeAll():
WindowNextPane():
WindowNextTab():
WindowPrevTab():